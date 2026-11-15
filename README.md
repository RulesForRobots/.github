# .github

The defaults for every repository in the RulesForRobots organization, and its front page.

| Path | What it is |
|---|---|
| `profile/README.md` | The organization's front page on GitHub |
| `brand/` | The marks, lockups, social previews, and colours of every volume, and the generator that writes them. See [brand/README.md](brand/README.md) |
| `CONTRIBUTING.md`, `SECURITY.md` | Used by every repository that has none of its own |
| `.github/ISSUE_TEMPLATE/`, `.github/pull_request_template.md` | The issue forms and pull request template, likewise |

A repository that adds its own file of one of these kinds stops using the default for that kind, so prefer changing the default here.

Verify: `npm run verify` checks that the brand's SVG files match `brand/tokens.json` and `brand/build.mjs`. Node 22 or later; no install step.
