# tabana plaja

Welcome to this project! Tabana is a payment orchestrator on Stellar.

## Setup

Install dependencies:

```bash
bun install
```

# Development

You can start working on the project by editing files inside `app/` directory.

# Code Quality

We care about keeping the code clean and consistent. Here's what We use:

- _Prettier_ for code formatting (e.g., spacing, quotes, etc.)
- _ESLint_ for finding common code issues
- _Husky_ for running checks automatically before commiting the code

## Pre-commit

Before each commit, Husky runs a check using Prettier and ESLint. If your commit is blocked, that means something needs fixing - probably formatting or a lint error.
You can fix most issues by running:

```bash
bun run lint     # Run ESLint
bun run format   # Run Prettier
```

# Contributing

Thank you for showing the interest in contributing; welcome! Fix that issue (type, or even add a feature!)

### Before you commit:

Please run the following commands:

```bash
bun run lint
bun run format
```

This checks for issues and formats your code to match our style.

⚠️ Running `prettier --write .` will format everything, which might take some time when(if) our project grows.
You might want to format specific files instead:

```bash
# Format a folder
prettier --write app/

# Format one file
prettier --write app/components/Button.js

# Format all tests in a folder using a glob
prettier --write "app/**/*.test.js"
```

See [fast-glob](https://github.com/mrmlnc/fast-glob#pattern-syntax) for more about glob syntax.

## Versioning and Releases

We use [changesets](https://github.com/changesets/changesets) to manage versions and changelogs across all our apps, and packages.

The project follows [Semantic Versioning](https://semver.org/) (SemVer), which means each change will bump the version as:

- **Patch:** small fixes (e.g., bugfixes, docs)
- **Minor:** new features that don’t break anything
- **Major:** breaking changes

The relevant folders that the changesets applies are in the "apps/\*" folder (soroban, metrics ...).

If your PR modifies any of the above, run

```bash
bunx changeset
```

Follow the prompts(pick version bump, write a short summary), and after this, a `.md` file will be created in the `.changeset/` folder.

When you're ready to apply the versions and changelogs, you can run:

```bash
bunx changeset version
```

That's it! See detailed info in the [changesets docs](https://github.com/changesets/changesets).

## 🫡 Thanks to Our Contributors

<a href="https://github.com/akkuea/tabana-plaja/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=akkuea/tabana-plaja" />
</a>

Made with [contrib.rocks](https://contrib.rocks).

We’re grateful for every contribution that brings us closer to what we're trying to achieve! 🙌

# License

This project is under the MIT License
