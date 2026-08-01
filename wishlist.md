# TUF Wishlist for Funders and Contributors
This is a wishlist of projects in the TUF ecosystem that could be taken on by funders or contributors looking to help the project. It consists of large feature requests that go beyond simple bug fixes and features. These features require a larger investment in engineering time, but can improve the adaptability, usability, and security of projects in the TUF ecosystem. Many, but not all, projects have associated Github issues where discussion can take place. For other projects please reach out to maintainers on Github or through the cncf slack.

## Go-tuf-metadata audit
The go-tuf project is planning a transition to a new codebase we’re calling “go-tuf-metadata”. This new codebase is based on the python-tuf re-write and is designed to improve the maintainability of go-tuf. As it is a new codebase, it would benefit from external security review.

## New threat model
The TUF project is designed to protect against a variety of [attacks](https://theupdateframework.io/security/). However, it is not always clear to newcomers which features of TUF protect against each attack. A new threat model and security analysis for TUF could make this relationship more clear. This security analysis could be expanded using formal methods to model the parties in TUF. [Related issue](https://github.com/theupdateframework/specification/issues/271).

## Specification clarity
The prose in the TUF specification is tricky to maintain as changes need to be made to multiple sections of the document. Further, as more TAPs are accepted, we need a way to include them in the specification without overwhelming the reader. As a community we have discussed making some TAPs optional in the specification so that not all implementations need to support them. However, there is currently no way for this optionality to be reflected in the specification. To solve these problems, we need to re-write the specification in a format that reduces duplication and allows for optional additions. [Some ideas for such a format have been proposed](https://github.com/theupdateframework/specification/issues/121).

## Cross implementation testing
Some TUF users would like interoperability across TUF implementations so that metadata created with one implementation can be verified using a client from a different implementation. To ensure that implementations remain compatible, we need interoperability testing. One plan for such testing is described [here](https://docs.google.com/document/d/11bKcRoC0G8b_YnLfK0tj1RfJjrMfXGhO8Li2LA1FUUk/edit#heading=h.w74e7wi8dmnz).

## TUF FFI
There are TUF implementations in python, go, rust, php, and more, each of which contains a full implementation of TUF. These implementations are in various states of maintainership, with some projects mostly unmaintained and others very active. To save on the overall maintenance requirements for TUF implementations, we could develop a shared library for most required functionality with small wrappers for each supported language using [FFI](https://en.wikipedia.org/wiki/Foreign_function_interface). There is a [related idea for the Sigstore project](https://docs.google.com/document/d/1cFJ_0cru99RupWS3VUJD6zmjzqXOoTUZ9Y0ugMXEK_o/edit) that could serve as a reference for this effort.

## Uptane example repository
The Uptane project has an example client implementation as part of Aktualizr. This project involves creating a ready to use repository that can be used with this client for those interested in experimenting with Uptane. Aktualizr contains test cases that rely on a sample repository. This repository could be expanded with CLI options to allow for such experimentation without requiring the setup of a full Uptane implementation.

## RSTUF + RubyGems integration
[Context](https://cloud-native.slack.com/archives/C047L55314N/p1690808447236489)

The [RSTUF](https://github.com/repository-service-tuf/repository-service-tuf) project mitigates many of the deployment challenges that have made doing this on the repository end so difficult in the past, and RubyGems is interested in deploying TUF using RSTUF. RubyGems maintainers are ready to offer support. This would be one of the largest-scale TUF deployments to date.

