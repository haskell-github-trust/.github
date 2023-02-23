# Haskell Library Trust

Haskell Library Trust is a Github organization for community ownership of Haskell libraries.

This is a place to store your Haskell libraries after you lose enthusiasm for maintenance.
You will still retain ownership and control of your library, but if you ever stop maintaining your library then by
default it will be publicly available for someone else to maintain.

The motivation is to reduce the difficultly for volunteers to maintain other people’s libraries.

The current situation is that if I see a library on Hackage which needs an update and I want to do the update myself,
I must email the author and ask to be added to the list of Hackage maintainers. In theory this seems like a good system,
but in practice it seems like that’s too much trouble, because there are a lot of useful libraries which are broken for want
of simple updates. By collecting libraries in this trust, we hope to encourage volunteer maintenance.

## How to add libraries to the Haskell Library Trust

1. Transfer Github ownership to https://github.com/haskell-library-trust
2. Add `haskell-library-trust` as a Hackage maintainer.

All libraries should have 

1. Names of authors and maintainers in README or .cabal file. Ways to contact.

If a library has an active maintainer, then any volunteer library improvements should be submitted as Pull Requests. If a library has been abandoned,
then any Trustee may make improvements, publish new versions, or take over as a maintainer. Use courtesy and judgement when deciding whether
a library has been abandoned.

## How to become a Trustee

Request to become a Trustee on Discussion page, or by asking any other Trustee. Trustees must be vouched for by one other trustee.
We keep a record of which trustees were vouched for by whom.
If any trustee 

* Uses the __haskell-library-trust__ CI to mine Bitcoin
* Inserts clandestine Bitcoin mining code in a library
* Deliberately weakens the security of a library to introduce Bitcoin ransomware vulnerabilities
* Uses the name of the __haskell-library-trust__ to sell Bitcoin-related services
* Or any other similar non-Bitcoin-related activity

then the trustee who vouched for them will be publicly blamed.

## How to add a Trustee

Any Trustee may add another person as a Trustee. Invite the other person to join the Github organziation, then add their name to the Trustee list and your own name as the Trustee who vouched for them. Every Trustee has full permission add repositories, to transfer repositories, to change repositories, and to publish packages to Hackage.

## How to quit being a Trustee

You can transfer your repos back to your own account and quit this organization any time you want.
