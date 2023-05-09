# Haskell GitHub Trust

Haskell GitHub Trust is a GitHub organization for community ownership of Haskell packages.

The essential feature of the Haskell GitHub Trust is that the Trust has a 
Hackage account
[haskell_github_trust](https://hackage.haskell.org/user/haskell_github_trust)
which has permission to publish any package in the Trust to Hackage.

This is a place to store your Haskell packages after you lose enthusiasm for maintenance.
You will still retain ownership and control of your package, but if you ever stop maintaining your package then by
default it will be publicly available for someone else to maintain.

The motivation is to reduce the difficulty for volunteers to maintain other people’s packages.

The current situation is that if I see a package on Hackage which needs an update and I want to do the update myself,
then I email the author and ask to be added to the list of Hackage maintainers. In theory this seems like a good system,
but in practice it seems like that’s too much trouble, because there are a lot of useful packages which are broken for want
of simple updates. By collecting packages in this trust, we hope to encourage volunteer maintenance.

## How to add packages to the Haskell GitHub Trust

1. Transfer GitHub ownership of the package repository to this organization, https://github.com/haskell-github-trust
2. Add https://hackage.haskell.org/user/haskell_github_trust as a Hackage maintainer for the package.

That’s it. We accept all packages, in any condition, with zero commitment or obligation.

## How to become a Trust Owner

Request to become a Trust Owner on Discussion page, or by asking any other Trust Owner. Trust Owners must be vouched for by one other Trust Owner.
We keep a [record of which Trust Owners were vouched for by whom](https://github.com/haskell-github-trust/.github/blob/main/TRUSTEES.md).

Every Trust Owner is an Owner of the __haskell-github-trust__ organization, so every Trust Owner can

* Transfer repositories in and out of the organization.
* Publish packages to Hackage via [haskell_github_trust](https://hackage.haskell.org/user/haskell_github_trust) account Authenticantion Token.

If any Trust Owner

* Inserts malevolent code in a package
* Uses the __haskell-github-trust__ for fraud
* Uses the __haskell-github-trust__ CI to mine Bitcoin
* Transfers a package repository without permission of the maintainer
* Or any other similar bad-faith activity

then that person and the Trust Owner who vouched for them will be publicly blamed.

## How to add a Trust Owner

Any Trust Owner may add another person whom they trust to be a Trust Owner. Invite the other person become an Owner of this GitHub organization, then add their name to the [Trust Owner list](https://github.com/haskell-github-trust/.github/blob/main/TRUSTEES.md) and your own name as the Trust Owner who vouched for them. Every Trust Owner has full permission to add repositories, to transfer repositories, to change repositories, and to publish packages to Hackage. For transparency, every Trust Owner should be a [__Public Owner__](https://github.com/orgs/haskell-github-trust/people) of the GitHub organization.

## How to quit being a Trust Owner

You can transfer your repos back to your own account and quit this organization any time you want.

## Package manners

If a package has an active maintainer, then any volunteer improvements should be submitted as Pull Requests.

If a package is being ignored,
then any Trust Owner may make improvements, publish new versions, or take over as a maintainer. Use courtesy and judgement when deciding whether
a package is being ignored.

## How to publish to Hackage

WIP

## How to take over a package

Follow the instructions in [Taking over a package](https://wiki.haskell.org/Taking_over_a_package) with the
Hackage account [haskell_github_trust](https://hackage.haskell.org/user/haskell_github_trust).

## Secrets

Every Trust Owner is an Owner of the __haskell-github-trust__ organization and has total control. The only restricted secrets are the passwords for the Hackage [__haskell_github_trust__](https://hackage.haskell.org/user/haskell_github_trust) account and the email account. These are stored in a separate organization https://github.com/haskell-github-trust-secrets

## Other organizations

* https://github.com/haskell-pkg-janitors Haskell package maintenance organization, but they don't publish a method for joining the org or adding libraries.
* https://github.com/haskell-party/ Haskell package maintenance organization, but they don't publish a method for joining the org or adding libraries. [Introducing Haskell Party proposal](https://github.com/haskellfoundation/stability/pull/12)
* https://github.com/rowtype-yoga PureScript “anarcho type-level collective”. Is the model for the Haskell GitHub Trust.

## FAQ

* Q. If someone upgrades my repo and publishes a release to Hackage while I'm on vacation, should I get offended?
  
  A. No. If they did something wrong then fix it and then publish another release.
  
* Q. What should I do if I suspect a Trust Owner is acting in bad faith?

  A. Talk about it in private messages with the other Trust Owners.

* Q. What happens if one of the Trust Owners transfers all the repos to the Trust Owner’s private account?

  A. We can fork the repositories back here and expel the Trust Owner.
  
* Q. What happens if one of the Trust Owners inserts security vulnerabilities and publishes to Hackage?

  A. This org has a Hackage Authentication Token, but not the Hackage password or email account. So we can revoke the Authentication Token and expel the Trust Owner.
