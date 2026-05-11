# Contributing To This Project

First off, thank you for considering contributing to the `Stablecoin Payment Plugin`. It is people
like you that make the open-source community such an amazing place to learn, inspire, and create.

All types of contributions are encouraged and valued. See the
[Table of Contents](#table-of-contents) for different ways to help and details about how this
project handles them. Please read the relevant section before making your contribution. It will make
things easier for maintainers and smoother for everyone involved.

> If you like the project but do not have time to contribute, that is fine too. Other helpful ways
> to support the project include:
>
> - Star the project
> - Share it with builders working on stablecoin payments
> - Reference it in your project's README
> - Mention it at meetups or in developer communities

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [I Have a Question](#i-have-a-question)
- [I Want To Contribute](#i-want-to-contribute)
- [Reporting Bugs](#reporting-bugs)
- [Suggesting Enhancements](#suggesting-enhancements)
- [Your First Code/Documentation Contribution](#your-first-codedocumentation-contribution)
- [Improving Documentation](#improving-documentation)
- [Styleguides](#styleguides)
- [Commit Messages](#commit-messages)

## Code of Conduct

This project and everyone participating in it is governed by the
[Stablecoin Payment Plugin Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected
to uphold this code. Please report unacceptable behavior to
[okpainmoandrew@gmail.com](mailto:okpainmoandrew@gmail.com).

## I Have a Question

> If you want to ask a question, we assume that you have read the available
> [documentation](README.md).

Before you ask a question, search existing
[issues](https://github.com/Okpainmo/stablecoin-payment-plugin/issues) that might help you. It is
also worth searching the internet or relevant ecosystem docs first.

If you still need clarification:

- Check the issue templates in [.github/ISSUE_TEMPLATE](.github/ISSUE_TEMPLATE).
- Open an [issue](https://github.com/Okpainmo/stablecoin-payment-plugin/issues/new).
- Provide as much context as you can about what you are running into.
- Include relevant environment details, chain/network, wallet/provider, contract version, SDK
  version, or a reproducible example when possible.

## I Want To Contribute

> ### Legal Notice
>
> When contributing to this project, you must agree that you authored 100% of the content, that you
> have the necessary rights to the content, and that the content you contribute may be provided
> under the project license.

### Reporting Bugs

#### Before Submitting a Bug Report

A good bug report should not leave others needing to chase more information. Please investigate
carefully, collect details, and describe the issue in enough depth for someone else to reproduce it.

- Make sure you are using the latest version available.
- Determine whether the problem is a project bug or an integration/configuration issue.
- Search the
  [bug tracker](https://github.com/Okpainmo/stablecoin-payment-plugin/issues?q=label%3Abug) for
  similar reports.
- Collect information about your stack:
  - OS and version
  - Runtime/tool versions
  - Chain/network and contract addresses, when safe to share
  - Wallet/provider or RPC details, when relevant
  - A reduced reproduction case, if possible

#### How Do I Submit a Good Bug Report?

> Do not report security vulnerabilities or sensitive information through public issues. See
> [SECURITY.md](SECURITY.md) instead.

We use GitHub issues to track bugs and errors. If you run into an issue:

- Open an [issue](https://github.com/Okpainmo/stablecoin-payment-plugin/issues/new).
- Explain the expected behavior and actual behavior.
- Provide reproduction steps someone else can follow.
- Include the information you collected in the previous section.

Once the issue is filed:

- The project team will label it accordingly.
- A maintainer may ask for reproduction steps and mark the issue as `needs-repro`.
- If the issue is reproduced, it may be marked `confirmed` and opened up for implementation.

### Suggesting Enhancements

This section guides you through submitting enhancement suggestions for Stablecoin Payment Plugin,
including new features and improvements to existing behavior.

#### Before Submitting an Enhancement

- Make sure you are using the latest version.
- Read the [documentation](README.md) and module READMEs to confirm the functionality is not already
  covered.
- Search [issues](https://github.com/Okpainmo/stablecoin-payment-plugin/issues) to see if the
  enhancement has already been suggested.
- Consider whether the idea fits the project's scope: vendor-agnostic, multi-chain, stablecoin
  payment rails that developers can own end to end.

#### How Do I Submit a Good Enhancement Suggestion?

Enhancement suggestions are tracked as
[GitHub issues](https://github.com/Okpainmo/stablecoin-payment-plugin/issues). The
[feature request template](.github/ISSUE_TEMPLATE/feature_request.md) is there to help.

- Open an [issue](https://github.com/Okpainmo/stablecoin-payment-plugin/issues/new).
- Use a clearly descriptive title.
- Describe the current behavior and the behavior you want to see.
- Explain why the enhancement would be useful to most users of the project.
- Mention related tools, protocols, or libraries that can serve as useful references.

### Your First Code/Documentation Contribution

#### Setup

Please follow the instructions in [README.md](README.md) and the relevant module README for project
prerequisites and environment setup.

We use Husky, Commitlint, and Prettier to keep contribution quality consistent. After cloning the
repo, run:

```bash
bun install
```

This sets up the git hooks required for local development.

#### Workflow

1. Fork the repo and create your branch from `main`.

> All contributions should come from a branch named in this format: `<preferred_code_name>_dev`, all
> lowercase.
>
> Example: `okpainmo_dev`

2. If you add code that should be tested, add tests.
3. If you change APIs, contracts, interfaces, configuration, or integration flow, update the docs.
4. Run the checks relevant to the modules you touched.
5. Make sure markdown formatting passes:

```bash
bun run format:check
```

### Improving Documentation

Documentation improvements are very welcome. If you find a typo, a confusing section, missing setup
details, or unclear integration steps, open a PR.

## Styleguides

### Markdown Formatting

We use Prettier for markdown formatting:

```bash
bun run format
```

### Project Checks

Run the tests and linting commands for any module you changed. For example, smart contract changes,
backend interaction changes, and Mesh integration changes may each have their own local verification
flow.

## Commit Messages

Use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) for commit messages and
PR titles.

Examples:

```text
feat(evm): add settlement adapter
fix(solana): handle missing token account
docs(mesh): clarify webhook setup
```
