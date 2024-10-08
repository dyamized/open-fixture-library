# Documentation Overview

This is the developer documentation for the *Open Fixture Library*. Please follow links in the folder structure below to get more information on a specific topic.

## Repository folder structure

* `cli/` – Useful scripts to be called from the command line
* `docs/` – Documentation (*you are here!*)
* `fixtures/` – Repository of our [fixture definitions](fixture-format.md)
* `lib/` – Reusable modules used in the project
  - `fixture-features/` – [Fixture features](fixture-features.md), special fixture characteristics used to determine a set of test fixtures
  - `model/` – Classes of the [fixture model](fixture-model.md) that help ease processing fixture data (see the [model API reference](model-api.md))
* `plugins/` – [Plugins](plugins.md) for export / import to / from other software's fixture formats
* `resources/` – Resources (e.g. [gobos](fixture-format.md#gobo-resources)) that fixtures can use
* `schemas/` – Schemas for the [fixture definitions](fixture-format.md#schema)
* `server/` – Load balancer config and auto-deploy script for everyone interested
* `tests/` – [Unit tests](testing.md), many of them run automatically in GitHub Actions
  - `github/` – Special kind of tests which shouldn't be called manually and create comments in GitHub pull requests
* `ui/` – Everything related to the [UI / Website](ui.md) (see docs there for subfolders)
* `tmp/` – Temporary files autogenerated by tests. Safe to delete and not indexed by Git.

## Local installation

### Linux / macOS

Make sure you have these dependencies installed:

* `git`
* [Node.js](https://nodejs.org/en/download/package-manager/)

Then run

```sh
git clone https://github.com/OpenLightingProject/open-fixture-library.git
cd open-fixture-library
npm install
npm run build
```

Continue with [UI docs](ui.md).

### Windows

Make sure you have these dependencies installed:

* [Git](https://gitforwindows.org/)
* [Node.js](https://nodejs.org/en/download/)
  * On the *Tools for Native Modules* page, activate the checkbox *Automatically install the necessary tools. [...]*

Choose a project path that only contains ASCII characters and no spaces. Open a Terminal and run

```bat
git clone https://github.com/OpenLightingProject/open-fixture-library.git
cd open-fixture-library
npm install
npm run build
```

Continue with [UI docs](ui.md).

## Contributing

Please see [`CONTRIBUTING.md`](CONTRIBUTING.md).

## Environment variables

See [`environment-variables.md`](environment-variables.md).
