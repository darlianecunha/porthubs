# Port Hubs: Brazil and Europe

**Port activity in Brazil (ANTAQ berthings) and Europe (Eurostat vessel arrivals), 2019-2025, each shown in its own metric and compared only where the comparison is valid: as an indexed trend (2019 = 100)**

[![Live site](https://img.shields.io/badge/Live-porthubs.vercel.app-2ea44f)](https://porthubs.vercel.app)
[![Part of Brazil Port Data](https://img.shields.io/badge/Part%20of-brazilportdata.com-0b2239)](https://www.brazilportdata.com)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

## What this is

Brazilian and European port statistics are often put side by side, but they do not count the same thing. ANTAQ records every berthing at every Brazilian installation, including inland navigation and support vessels; Eurostat counts arrivals of vessels of 100 GT and over at the main ports of each country. This page keeps the two sources in separate tabs, each in its own unit, and brings them together only in an index that shows each series against its own 2019 level.

| Indicator (2019 → 2025) | Brazil, all installations | Brazil, public ports only | Europe, 24 countries |
|---|---|---|---|
| 2019 | 65,079 berthings | 26,089 berthings | 2,398,057 arrivals |
| 2025 | 94,104 berthings | 32,810 berthings | 2,330,964 arrivals |
| Change | **+44.6%** | **+25.8%** | **-2.8%** |

In Brazil, growth is concentrated in the North (+55.2%, led by Pará and Amazonas, mostly inland navigation) and the Southeast (+81.0%). In Europe, Greece, Italy, Denmark and Croatia lead on arrival counts because of ferry traffic, not cargo volume.

## What the page shows

| Tab | Content |
|---|---|
| **Brazil (ANTAQ)** | Berthings by region in 2025, change since 2019 per region, and a breakdown by state (UF). A filter switches between all installations and public ports only |
| **Europe (Eurostat)** | Arrivals by country in 2025 and change since 2019 |
| **Comparison (trend)** | Both series indexed to 2019 = 100, with the growth gap between Brazil and Europe |

## Method notes

- **Brazil:** ANTAQ *Estatístico Aquaviário*, berthings by installation, aggregated by region and state. Closed calendar years.
- **Europe:** Eurostat dataset `mar_tf_qm` (vessels arriving in the main ports), summed by country.
- **Same countries in every year.** The European total uses the 24 countries with data for every year from 2019 to 2025. The United Kingdom (no Eurostat data after 2019) and Cyprus (no 2025 data) are left out; including them would mix different sets of countries across years and overstate the European decline (-7.0% instead of -2.8%).
- **Levels are not comparable.** A Brazilian berthing and a European arrival are different units with different coverage. Only growth rates should be compared.
- **Limitations:** regions are Brazil's five macro-regions, not port hubs in the logistics sense; national totals for Europe are dominated by ferry and short-sea traffic in some countries.

## Repository map

| Path | Content |
|---|---|
| `index.html` | The whole application: page, aggregated data and charts (Chart.js) in one file |

The aggregated series are embedded in the page. Underlying installation-level data are not published in this repository; annual ANTAQ tables are available in the open dataset [Brazil Port Data](https://doi.org/10.5281/zenodo.23158267).

## Related projects

- [brazilportdata](https://github.com/darlianecunha/brazilportdata): the hub site that links this and the other Brazilian port panels
- [antaq-port-statistics](https://github.com/darlianecunha/antaq-port-statistics): open dataset of annual ANTAQ port statistics, 2010-2026
- [port-traffic-explorer](https://github.com/darlianecunha/port-traffic-explorer): European port arrivals by ship type and size class (Eurostat)
- [vessel-gigantism](https://github.com/darlianecunha/vessel-gigantism): three decades of "fewer ships, bigger ships" in European ports

## Author and licence

**Darliane Ribeiro Cunha, PhD**. [ribeirocunha.com](https://ribeirocunha.com) · [ORCID 0000-0003-2548-1237](https://orcid.org/0000-0003-2548-1237)

Analysis and page: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Sources: ANTAQ (Brazil) and Eurostat (European Union), under their respective open-data terms.
