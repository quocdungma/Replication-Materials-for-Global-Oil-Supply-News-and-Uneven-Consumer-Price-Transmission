# Data Availability and Access Restrictions

**Study:** *Global Oil Supply News and Uneven Consumer Price Transmission: Implications for Middle East Energy Risks*

**Repository status (17 October 2026):** This repository is in preparation. The repository now includes `README.md`, `DATA_AVAILABILITY.md`, `data_dictionary.csv`, `data_sources.csv`, 12 validated numerical result CSVs in `results/`, and the original three v6 manuscript figures in `figures/`. **Licensed CPI source observations, the analysis-ready panel, and executable replication scripts have not been deposited.** Do not describe this repository as a complete replication archive.

## 1. Data used in the empirical analysis

| Material | Source / provenance | Access and redistribution | Repository status |
| --- | --- | --- | --- |
| Monthly national headline CPI observations, 23 economies, 2000–2025 | LSEG/Refinitiv accessed under institutional arrangements | **Restricted.** Vendor-supplied observations are not publicly redistributed here. Researchers should arrange access directly with the data provider, subject to licensing. | Not deposited |
| Published monthly oil supply news shock measure | Published series associated with Känzig (2021), *The Macroeconomic Effects of Oil Supply News: Evidence from OPEC Announcements* | Third-party research data; consult the author's release and applicable reuse terms. The shock is used as published; it was not re-identified in this project. | Source documented; underlying series not deposited |
| Historical GDP and GDP per capita moderators | Maddison Project historical economic data, summarized over the predetermined baseline period | Third-party data; precise release, citation, and permitted download location must be recorded before any redistribution. | Source documented; underlying observations not deposited |
| Energy-exposure and regional moderators | Sources identified in the study's data collection workflow and manuscript | Variable-specific provenance, transformations, coverage, and reuse permissions require verification and documentation. | Not deposited |
| 2026 Brent/WTI price series and Middle East energy-market chronology | External sources including U.S. EIA and IEA, cited in the manuscript | Descriptive **post-estimation context only**. The 2026 observations are **not** included in the 2000–2025 CPI local-projection estimation sample. | Not deposited |

### Third-party source references

- Känzig, D. R. (2021). *The Macroeconomic Effects of Oil Supply News: Evidence from OPEC Announcements*. *American Economic Review*, 111(4), 1092–1125. https://doi.org/10.1257/aer.20190964
- Maddison Project data portal (historical national accounts): https://www.rug.nl/ggdc/historicaldevelopment/maddison/ . **The exact version used in the regressions must be specified in the data-source manifest before release.**
- LSEG data access: https://www.lseg.com/ . Access and permitted uses depend on the relevant subscription/licensing arrangements.
- U.S. Energy Information Administration, petroleum spot-price data: https://www.eia.gov/dnav/pet/pet_pri_spt_s1_m.htm (contextual analysis, not a substitute for the news-shock series).

Links identify providers or source studies; they do not imply that this repository redistributes or licenses their data.

## 2. Why CPI source observations are not public

The underlying CPI observations were retrieved through a commercial LSEG/Refinitiv data service. Public repository access does not grant a right to redistribute the licensed observations, including extracted workbooks or an analysis-ready panel that reproduces the vendor's licensed series.

Researchers seeking access to equivalent observations should request access from the original data provider or identify an independently licensed public source. A request to this repository's maintainer does **not** override LSEG/Refinitiv licensing rules. No claim is made that the author can directly supply restricted input data upon request.

## 3. Research-generated documentation and materials

**Already available:** `README.md`, this data-access policy, `data_dictionary.csv`, a provisional `data_sources.csv` with 23-country coverage and *unverified* candidate CPI RICs, 12 v6–v7 result tables, and the original three v6 image files. Fields requiring code-level or data-source verification are explicitly flagged in the dictionary and source manifest.

**Planned for future deposit:** Subject to checking provenance, numerical fidelity, and redistribution rights, the project intends to deposit:

- A data-source manifest identifying the economies, CPI-series identifiers, date coverage, missing-data handling, and specific versions of public inputs.
- Complete figure-source data beyond what is contained in the currently deposited result tables.
- The final Figure 4 on the 2026 oil context, after provenance and version checks.
- The original model-estimation, bootstrap, and plotting scripts, after they are located and independently verified against reported results.
- A record of the software environment and instructions for running the scripts with appropriately licensed input data.

**None of these planned files should be cited as deposited until visible in the repository and verified against the paper.** Analytical outputs derived from restricted sources will be reviewed before posting; outputs are not assumed automatically free of contractual restrictions.

## 4. Reproducibility and scope

The analysis covers 23 economies from January 2000 through December 2025, although each regression uses fewer effective observations because of lagged controls and horizon-specific forward CPI outcomes. The main regressor is the published monthly Känzig oil supply news *shock measure*, not a percentage change in Brent/WTI and not the original high-frequency instrument.

Any replication of the reported coefficients requires matching the original country CPI definitions, sample filters, monthly alignment, shock standardization, local-projection specifications, and inference settings. Reproduction from publicly available outputs alone is **not equivalent to independently re-estimating the model from the restricted CPI observations**.

The 2026 Middle East war and energy price developments are discussed as external context, not treated as model-estimated oil supply news shocks or used for causal forecasts of 2026 CPI.

## 5. Data Availability Statement (final wording for the current repository contents)

The national consumer price index (CPI) observations used in this study were accessed through LSEG/Refinitiv under institutional data-access arrangements. These proprietary observations are subject to third-party licensing restrictions and cannot be redistributed publicly by the authors. Researchers wishing to obtain the underlying CPI observations should seek access directly from the data provider under the applicable licensing terms. The published oil supply news shock series and historical economic characteristics were obtained from the third-party sources cited in the manuscript. Research documentation, a data dictionary, a provisional source manifest, selected empirical-result tables, and the three original core manuscript figures are publicly available at **https://github.com/quocdungma/Replication-Materials-for-Global-Oil-Supply-News-and-Uneven-Consumer-Price-Transmission**. The repository does not contain proprietary CPI observations, the complete analysis-ready panel, or executable replication code. The candidate CPI identifiers in the source manifest still require verification against the final estimation dataset.

**Status clarification:** This statement accurately describes the repository *as currently published*. It is not a claim that a complete replication archive is available or that the journal has granted a commercial-data exemption. Update this statement if verified code or additional research material is deposited before submission; add a persistent archival DOI when one is actually issued.

## 6. Citation, reuse, and repository archiving

This is a public GitHub repository for documentation and permitted replication materials. **Public GitHub visibility does not establish a citable, permanent research-data deposit or provide a DOI.** A versioned release can be archived using a suitable research repository (for example, Zenodo) after the files have been audited. Until then, no permanent dataset identifier is claimed.

Licensing for *original code and documentation* will be considered separately from third-party input data and generated outputs. No license for proprietary LSEG/Refinitiv observations is granted here.

## 7. Remaining release checks

Before using this repository as the journal's data-deposition link, verify:

1. The journal's exact data-deposition policy and any acceptable provisions for proprietary datasets.
2. Whether the analysis-ready data or derived outputs include any vendor-restricted content.
3. Source series identifiers, historical coverage, missingness, and exact dataset versions.
4. Numerical reproduction of results and figures from the actual analysis code.
5. Public availability of the promised materials and, where applicable, a permanent archived DOI.

Questions concerning documentation can be raised via GitHub Issues; do not post credentials or restricted data in public issues.
