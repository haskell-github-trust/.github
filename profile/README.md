# Haskell GitHub Trust

Haskell GitHub Trust is a GitHub organization for community ownership of Haskell packages.

The two essential features of the Haskell GitHub Trust are

1. All Haskell Github Trust organization members are Owners, and have control over all repositories, including transferring in and out.
2. A Hackage “Group Account” [haskell_github_trust](https://hackage.haskell.org/user/haskell_github_trust) so that every Trust Owner can publish any package in the Trust.

This is a place to keep your Haskell packages for long-term community maintenance.

You will still retain ownership and control of your package, but if you ever stop maintaining your package then someone else can do it without needing your permission.

## How to add your own package to the Trust

1. Transfer GitHub ownership of the package repository to this organization, https://github.com/haskell-github-trust
2. Add https://hackage.haskell.org/user/haskell_github_trust as a Hackage maintainer for the package.

That’s it. We accept all packages, in any condition, with zero commitment or obligation.

## How to become a Trust Owner

Request to become a Trust Owner on the [Discussions](https://github.com/orgs/haskell-github-trust/discussions) page, or by asking any other Trust Owner. Trust Owners must be vouched for by one other Trust Owner.
We keep a [record of which Trust Owners were vouched for by whom](https://github.com/haskell-github-trust/.github/blob/main/TRUSTEES.md).

After you accept the Trust Owner invitation, [set your visiblity to __*Public*__](https://github.com/orgs/haskell-github-trust/people) for transparency.

If any Trust Owner

* Inserts malevolent code in a package
* Uses the __haskell-github-trust__ for fraud
* Uses the __haskell-github-trust__ CI to mine Bitcoin
* Transfers a package repository out of this org without permission of the maintainer
* Or any other similar bad-faith activity

then that person and the Trust Owner who vouched for them will be publicly blamed.

## How to add a Trust Owner

Any Trust Owner may add another person whom they trust to be a Trust Owner. [Invite](https://github.com/orgs/haskell-github-trust/people) the other person to become an Owner of this GitHub organization, then add their name to the [Trust Owner list](https://github.com/haskell-github-trust/.github/blob/main/TRUSTEES.md) and your own name as the Trust Owner who vouched for them. For transparency, every Trust Owner should be a [__*Public*__ Owner](https://github.com/orgs/haskell-github-trust/people) of the GitHub organization.

## How to publish to Hackage

You need your own “uploader” account on Hackage. Use the [__haskell_github_trust__ account password](https://github.com/haskell-github-trust/secrets) 
to add your own “uploader” account to the list of package Maintainers.
The __haskell_github_trust__ account does not have upload permission, rather it is a “Group Account” as described
on [hackage.haskell.org/upload](https://hackage.haskell.org/upload).

> #### Group Accounts
> 
> Occasionally organizations want to have a group / organizational account for a package that is maintained by a group of people. The recommended approach for these cases is to only do package uploads from individual accounts and use the group account only for managing the maintainer list for the package.

In this way you can [upload](https://hackage.haskell.org/upload) any package in this org.

## How to add other people’s packages to the Trust

1. Follow the instructions in [Taking over a package](https://wiki.haskell.org/Taking_over_a_package) with your own Hackage account. Declare your intent to add the package to the Haskell GitHub Trust.
2. Add the Hackage account [haskell_github_trust](https://hackage.haskell.org/user/haskell_github_trust) to the list of package Maintainers.
3. Transfer or fork the package repository into this org.

## How to talk about the Haskell Github Trust

Talk in the [GitHub Discussions](https://github.com/orgs/haskell-github-trust/discussions) or in [Haskell Discourse](https://discourse.haskell.org/).

## How to quit being a Trust Owner

You can transfer your repos back to your own account and quit this organization any time you want.

## Package manners

If a package has an active maintainer, then any volunteer improvements should be submitted as Pull Requests.

If a package is being ignored,
then any Trust Owner may make improvements and publish new versions. Use courtesy and judgement when deciding whether
a package is being ignored.

## Secrets

The password for the __haskell_github_trust__ Hackage account is in https://github.com/haskell-github-trust/secrets . 

The only restricted secret is the password for the email account used to create the __haskell_github_trust__ acount. This is stored in a separate organization https://github.com/haskell-github-trust-secrets

## Other organizations

* https://github.com/haskell-pkg-janitors Haskell package maintenance organization. [how to join this group?](https://github.com/orgs/haskell-pkg-janitors/discussions/3)
* https://github.com/haskell-party/ Haskell package maintenance organization. [Introducing Haskell Party proposal](https://github.com/haskellfoundation/stability/pull/12)
* https://github.com/haskell-works Also has a “Group Account” [haskellworks](https://hackage.haskell.org/user/haskellworks)
* https://github.com/rowtype-yoga This PureScript “anarcho type-level collective” is the model for the Haskell GitHub Trust.

## FAQ

* Q. If someone upgrades my repo and publishes a release to Hackage while I'm on vacation, should I get offended?
  
  A. No. If they did something wrong then fix it and then publish another release.
  
* Q. What should I do if I suspect a Trust Owner is acting in bad faith?

  A. Talk about it in private messages with the other Trust Owners.

* Q. What happens if one of the Trust Owners transfers all the repos to the Trust Owner’s private account?

  A. We can fork the repositories back here and expel the Trust Owner.
  
* Q. What happens if one of the Trust Owners inserts malicious code and publishes to Hackage?

  A. Talk to the Hackage Trustees.
  
* Q. What happens if a Trust Owner deletes this whole org?

  A. We can rebuild this org from local clones of the repositories. We would lose the information in the GitHub Issues.
     Nothing else would be lost.
