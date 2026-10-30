# Income Tax Slabs

Income tax slabs for old and new regime, by financial year

- **Base URL:** https://chirag127.github.io/income-tax-slabs-api/
- **Contract:** [openapi.yaml](./openapi.yaml)
- **Repository:** https://github.com/chirag127/income-tax-slabs-api

This is a static JSON API. No authentication, no server, and no rate limit. The committed JSON is the database.

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| `GET` | `/api/v1/data.json` | Income Tax Slabs |
| `GET` | `/api/v1/individual/{id}.json` | Get single record |
| `GET` | `/api/v1/search-index.json` | Search index |
| `GET` | `/api/v1/meta.json` | Dataset metadata |

## Data and metadata

The current record count, source, retrieval time, and schema version are published at [`/api/v1/meta.json`](https://chirag127.github.io/income-tax-slabs-api/api/v1/meta.json). The static data lives under `api/v1/`.

Data licensing: CC-BY-4.0. Code licensing: MIT. See `openapi.yaml` and the repository license for details.

## Local verification

```bash
ls api/v1
curl -s https://chirag127.github.io/income-tax-slabs-api/api/v1/meta.json
```
