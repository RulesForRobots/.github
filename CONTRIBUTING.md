# Contributing

Thank you for helping. This is the default guide for every repository in the RulesForRobots organization; a repository's own `AGENTS.md` adds what is particular to it.

## Where things go

- **Feedback from a project that uses Rules for Robots**: open an issue with the "Feedback from a project" form, on the repository of the plugin concerned, or let the `rfr-feedback` plugin's `report-feedback` skill draft it. If you are not sure which repository, use [rules-for-robots](https://github.com/RulesForRobots/rules-for-robots).
- **A change to a plugin**: a pull request on the repository that holds it. The [front door's README](https://github.com/RulesForRobots/rules-for-robots) lists the plugins and where each lives.
- **A security problem**: not an issue. See [SECURITY.md](SECURITY.md).

## Setup

Node 22 or later. Nothing to install: each repository's checks are Node scripts with no dependencies.

```
npm run verify
```

`npm run verify` runs what CI runs. Run it before opening a pull request, and paste its summary into the pull request.

## Pull requests

- One change per pull request, small enough to review in one sitting.
- Raise a plugin's `version` in its `plugin.json` when its contents change, and add the change to its `CHANGELOG.md` under `## Unreleased`.
- A plugin is self-contained: nothing outside its folder at run time. CI refuses a run-time reference outside it.
- A rule ships only with a mechanical check or evidence that it changes agent behaviour, and the evidence sits beside the rule.
- A file carried over from the archived repository (`lifelike-and-believable/rules-for-robots`) arrives in a commit whose message names its source path and commit.
- Specs say what is true now. Put the reasoning for a change in a decision record in `docs/decisions/`.

## Style

Canadian English. Plain sentences. Avoid emphatic capitals, frequent em dashes, and "it's not X, it's Y" constructions.
