# .github

The RulesForRobots organization's front page (`profile/README.md`), its brand (`brand/`), and the community files every repository uses unless it has its own: `CONTRIBUTING.md`, `SECURITY.md`, the issue forms, and the pull request template. The charter and the work across repositories are in [RulesForRobots/rules-for-robots](https://github.com/RulesForRobots/rules-for-robots).

## Commands

- Verify (run before reporting work as done, and include its output): `npm run verify`. It rebuilds the brand's SVG files and fails if they differ from what is committed.
- After changing `brand/tokens.json`, `brand/build.mjs`, or `brand/wordmarks.json`: `npm run brand`, which also renders the PNG files (needs Playwright with its Chromium). Never edit a generated file.

## Conventions

- A change to a default here changes it for every repository that has no file of its own. Say which repositories it affects in the pull request.
- The feedback form's field IDs must match `FIELDS` in the `rfr-feedback` plugin; change both together.
- Canadian English. Plain sentences; no emphatic capitals, few em dashes, no "it's not X, it's Y" constructions.
