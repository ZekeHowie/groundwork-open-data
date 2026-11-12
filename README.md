# Groundwork Map open data

Open tables from [Groundwork Map](https://groundworkmap.com/data), built from public records and published under CC BY 4.0. One table today:

| Table | Rows | Data as of | DOI |
|---|---|---|---|
| [florida-land-prices.csv](florida-land-prices.csv) ([JSON](florida-land-prices.json)) | 434 | 2026-11-01 | [10.5281/zenodo.24092813](https://doi.org/10.5281/zenodo.24092813) |

Also on [Hugging Face](https://huggingface.co/datasets/Zekehowie/florida-land-prices). Live copy, updated with the site: https://groundworkmap.com/data/florida-land-prices


## About Groundwork Map

[Groundwork Map](https://groundworkmap.com) is a free map of public land facts, parcel by parcel: 55.6 million parcels in 10 US states, built from county and state records, each fact shown with its source and date. Its open tables are listed at https://groundworkmap.com/data (machine-readable catalog: https://groundworkmap.com/data.json).

Copies of this table: [Zenodo](https://doi.org/10.5281/zenodo.24092813) (permanent DOI) and [Hugging Face](https://huggingface.co/datasets/Zekehowie/florida-land-prices). Contact: hello@groundworkmap.com

## Florida vacant-land prices by county and city

Median price per acre of arm's-length vacant-land sales of 1+ acre, with the sale count and the months the sales span, for every Florida county and city market page on groundworkmap.com. A blank median: fewer than 5 qualifying sales (the site page then shows a wider market's figure, labeled).

- **Rows:** 434
- **Data as of:** 2026-11-01
- **Source page:** https://groundworkmap.com/data/florida-land-prices (live copy, updated with the site)
- **Licence:** CC BY 4.0. Credit "Groundwork Map (groundworkmap.com)" and link the row's `page_url` or https://groundworkmap.com/data/florida-land-prices.
- **Publisher:** Groundwork Map, groundworkmap.com (Zeke Howie)
- **DOI:** [10.5281/zenodo.24092813](https://doi.org/10.5281/zenodo.24092813) (Zenodo, same files)
- **Contact:** hello@groundworkmap.com

## Columns

| Column | Meaning |
|---|---|
| `county` | County name |
| `city` | City name; blank on a county row |
| `page_url` | The Groundwork Map page that prints the row |
| `median_usd_per_acre` | Median price per acre (USD) of arm's-length vacant-land sales of 1 acre or more; blank under the minimum sale count |
| `n_sales` | Sales of 1 acre or more behind the median |
| `sale_date_min` | First month of the sales range the page prints (YYYY-MM) |
| `sale_date_max` | Last month of the sales range the page prints (YYYY-MM) |
| `size_band` | Size band of the per-acre median |
| `median_usd_per_lot` | Median price (USD) of vacant-lot sales under 1 acre |
| `n_lot_sales` | Vacant-lot sales under 1 acre |
| `as_of` | Data date of the row (YYYY-MM-DD) |
| `method` | How the median is computed |
| `source` | Source records |
| `license` | Licence of the row |

## Method

Median of arm's-length vacant-land sales of 1+ acre, USD per acre. Latest arm's-length sale per vacant parcel; one deed of several parcels counts once. $/acre over 1+ acre sales, per lot under 1 acre. Non-ag sales above 3× assessed value excluded (built on since the Jan 1 roll). Each county's 12 months end with its latest fully recorded month; Florida and region totals end with the month most counties have recorded.

## Terms

Free to copy, share and adapt, including commercially, under CC BY 4.0: credit "Groundwork Map (groundworkmap.com)" and link the row's page_url or https://groundworkmap.com/data/florida-land-prices. The license covers these files only; the rest of the site and the map stay under https://groundworkmap.com/terms. Aggregates of public records, not an appraisal. Groundwork Map is not affiliated with any county property appraiser or government.

Aggregates of public records only: no parcel identifiers, owner names, addresses or value estimates.

## Citation

Howie, Zeke (Groundwork Map). “Florida vacant-land prices by county and city” (2026-11-01). Zenodo. https://doi.org/10.5281/zenodo.24092813. Also at https://groundworkmap.com/data/florida-land-prices.

```bibtex
@dataset{howie_2026_florida_land_prices,
  author    = {Howie, Zeke},
  title     = {Florida vacant-land prices by county and city (2026-11-01)},
  publisher = {Groundwork Map},
  year      = {2026},
  version   = {2026-11-01},
  doi       = {10.5281/zenodo.24092813},
  url       = {https://doi.org/10.5281/zenodo.24092813}
}
```

## Licence

The data files are under [CC BY 4.0](LICENSE). Credit "Groundwork Map (groundworkmap.com)".
