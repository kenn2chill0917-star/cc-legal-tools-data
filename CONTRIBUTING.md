# Contributing to CC Open Source

Thank you for your interest in contributing to CC Open Source! This document is
a set of guidelines to help you contribute to this project.


## Code of Conduct

By participating in this project, you are expected to uphold our [Code of
Conduct][code_of_conduct].

[code_of_conduct]: https://opensource.creativecommons.org/community/code-of-conduct/


## Project Documentation

The `README` in the root of the repository should contain or link to project
documentation. If you cannot find the documentation you're looking for, please
file a GitHub issue with details of what you'd like to see documented.


### Evaluating External Code References

This repository stores source and generated data for Creative Commons legal
tools. Runtime and application source changes belong in
[`creativecommons/cc-legal-tools-app`][cc-legal-tools-app]. Before acting on a
reference to another codebase:

- identify whether it changes application behavior, source data, or generated
  artifacts
- trace generated files back to their source; do not copy them independently
- verify that the repository contains an applicable code or data surface
- redirect implementation work to the project that owns that surface rather
  than vendoring unrelated code here

For example, [the referenced ethers.js commit][ethers-dist-refresh] is an
`admin: updated dist files` release-artifact refresh. It updates ethers.js
distribution and version artifacts, not CC legal-tool data. This repository
has no ethers.js package or runtime integration, so the commit must not be
ported or vendored here.

[cc-legal-tools-app]: https://github.com/creativecommons/cc-legal-tools-app
[ethers-dist-refresh]: https://github.com/ethers-io/ethers.js/commit/3ea4c226dd0b3a074abf90748de9d11192027f4f


## How to Contribute

Please follow the processes in our general [Contributing Code][contributing]
guidelines on the Creative Common Open Source website.

[contributing]: https://opensource.creativecommons.org/contributing-code/


## Questions or Thoughts?

Talk to us on [one of our community forums][community].

[community]: https://opensource.creativecommons.org/community/
