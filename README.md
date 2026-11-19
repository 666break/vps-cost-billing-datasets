# VPS Cost & Billing Datasets

Machine-readable copies of the comparison tables published at [ServerBudget](https://serverbudget.com/), a site that documents what cheap VPS providers actually charge once a plan is in use: renewal, extra IPv4 addresses, snapshots, bandwidth overage, and backup versus restore.

Every CSV under `datasets/` is a verbatim copy of a table on a live page. The first two lines of each file name the exact source page and the dataset title. Figures in those tables were read from official provider documentation and carry a check date on the source page; this repository copies them as published and does not re-derive or update them. See [DATASETS.md](DATASETS.md) for the file index and source links.

## What is here

- `datasets/vps-price-per-gb-*.csv` — normalized price per vCPU, per GB RAM and per GB storage for entry and higher tiers.
- `datasets/extra-ipv4-pricing-*.csv` — monthly and hourly cost of additional IPv4 addresses, and the state each price applies to.
- `datasets/snapshot-billing-*.csv` — published snapshot rates, what is billed, minimums and proration, plus worked examples.
- `datasets/bandwidth-overage-*.csv` — included transfer and what happens past it, by provider and region.
- `datasets/backup-restore-verification-*.csv` — what three providers' official pages print about backup retention and restore testing.

## Use

These files are provided as-is for anyone who wants to cite or re-check the numbers without scraping HTML. If a figure is stale, consult the source page, which records the check date and the official link.

Data source: [serverbudget.com](https://serverbudget.com/).
