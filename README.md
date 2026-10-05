# Platform Requirements

What Claude, ChatGPT, Cursor and the Official MCP Registry require before they list an MCP connector or plugin, each requirement with its sources, evidence label and the date it was last checked, plus a dated log of platform changes.

Maintained by [Invokary](https://invokary.com/platforms). This repository mirrors the files published on invokary.com; a daily workflow copies them here when they change and tags each change `vYYYY.MM.DD`.

## Files

| File | What it holds |
|---|---|
| `platform-requirements.json` | Every requirement and every platform change note, with sources and dates |
| `platform-requirements.csv` | The requirements, one row per requirement |
| `platform-changes.csv` | The platform change notes, one row per note |
| `platform-requirements.schema.json` | JSON Schema (draft 2020-12) for the JSON file |

Each requirement has a stable `id` (for example `claude.rule-annotations`). An id is never reused; a requirement that is removed is listed under `retired`, with the requirement that replaces it if there is one. `schemaVersion` follows semantic versioning: a breaking change to a field bumps the major version.

Fields worth knowing:
- `evidence`: `V` verified against the platform's own documentation, `3P` third-party, `CC` company claim, `INF` inference.
- `sourceKind`: derived from the hosts of the sources, never typed by hand.
- `verifiedAt`: the date the requirement was last checked against its sources.
- `url`: the requirement's row on its platform page on invokary.com.

The same data is on [invokary.com/platforms](https://invokary.com/platforms), and every page of the site has a Markdown version at its URL plus `.md`.

## License

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Credit Invokary and link to https://invokary.com/platforms. See `CITATION.cff`.

## Corrections

Found a requirement that is out of date? Open an issue with the platform's page that says otherwise, or write to hello@invokary.com.
