# Setting up `semantic-release` for Haskell Github Trust packages

Once a version of your package has been uploaded to Hackage and the trust
account has been added to the maintainers, you can use the [semantic-release
action](https://github.com/cycjimmy/semantic-release-action) to publish new
versions automatically. The organization already has everything configured, you
only need to configure a few things.

In this example, we use the `stack-upload` plugin to upload to hackage, but feel
free to use the `cabal` actions if you don't like `stack`. We also use `main` as
the default branch, make sure to modify the snippets if you use a different
default branch name.

## Install the Github App on your repository
The first step is to add the [Github
app](https://github.com/organizations/haskell-github-trust/settings/installations/79745966)
to your repository by adding it to the selected repositories in `Repository access`.

## Configure `semantic-release` in your repository
In your repository at the root, configure `semantic-release` by adding the
`.releaserc.mjs` at the root:

```javascript
/**
 * @type {import('semantic-release').GlobalConfig}
 */
export default {
    branches: ["main"],
    tagFormat: "${version}",
    plugins: [
        "semantic-release-stack-upload",
    ]
}
```

## Add the `semantic-release` action to your repository
In your repository, in `.github/workflows/semantic-release.yaml`, include this snippet:

```yaml
---
name: Semantic release
on:
  push:
    branches:
      - main

jobs:
  build:
    name: Semantic release
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
        with:
          persist-credentials: false

      - uses: actions/create-github-app-token@v2
        id: app-token
        with:
          app-id: "${{ secrets.SEMANTIC_RELEASE_APP_ID }}"
          private-key: "${{ secrets.SEMANTIC_RELEASE_PRIVATE_KEY }}"

      - name: Semantic release
        id: semantic
        uses: cycjimmy/semantic-release-action@v4
        env:
          GITHUB_TOKEN: "${{ steps.app-token.outputs.token }}"
          HACKAGE_KEY: "${{ secrets.HACKAGE_TOKEN }}"

        with:
          ci: ${{ github.ref == github.event.repository.default_branch }}
          extra_plugins: |
            semantic-release-stack-upload
```
