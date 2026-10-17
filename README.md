# Replication Materials: Global Oil Supply News and Uneven Consumer Price Transmission

This repository is being prepared as supporting material for the manuscript:

**Global Oil Supply News and Uneven Consumer Price Transmission: Implications for Middle East Energy Risks**

**Repository status:** Initial setup. Public documentation, a provisional CPI-source manifest, verified summary regression-result CSVs, and the three original manuscript figures have now been deposited. **Licensed CPI observations and executable replication code have not been deposited.** The repository should not yet be described as a complete replication package.

## Research overview

The study examines dynamic consumer price index (CPI) responses to the **published oil supply news shock measure associated with Känzig (2021)** in 23 economies, using monthly data for **January 2000–December 2025**.

The empirical design includes:

- Pooled and economy-specific local projections of cumulative log-CPI changes at horizons 0–24 months.
- Heteroskedasticity- and autocorrelation-consistent (HAC) inference that accounts for common monthly disturbances.
- Joint Wald tests of equality of country-specific shock responses.
- Conditional moving-block score bootstrap and leave-one-country-out sensitivity checks.
- Exploratory interaction analyses involving predetermined economic size, development, and energy-exposure indicators.

These analyses condition on the published shock series and the original study's structural identification assumptions.

## Data sources and access restrictions

- **National CPI:** Accessed through LSEG/Refinitiv under data-access arrangements. The underlying vendor-supplied observations may be subject to contractual redistribution restrictions and **are not included in this public repository**.
- **Oil supply news measure:** Based on the published series associated with Känzig (2021); see the source study at https://doi.org/10.1257/aer.20190964. Source links, versions, and permitted access methods will be documented separately.
- **Historical economic characteristics:** Drawn from the sources specified in the manuscript, including the Maddison Project for economic size and development.
- **2026 Middle East oil-market events:** Used as external discussion context only; **not** part of the 2000–2025 estimation sample.

Researchers seeking proprietary CPI observations should consult the original provider and its licensing requirements. This repository does not grant redistribution rights to third-party datasets.

## Planned repository materials

The file structure below distinguishes **available** documentation/results from **planned** files:

```text
README.md                   # Available
DATA_AVAILABILITY.md        # Available
data_dictionary.csv         # Available
data_sources.csv            # Available (provisional CPI ticker candidates; not final-code verified)
results/                    # Available (v6-v7 published empirical summaries)
figures/                    # Available (three original v6 figures; not the 2026 context Figure 4)
code/                       # Planned
requirements.txt            # Planned
```

Where source data can lawfully be shared, the project aims to include verified analytical outputs, figure data, documented code, and sufficient instructions to reproduce the reported calculations with independently obtained licensed input data.

## Verified analytical outputs available

The `results/` folder contains the following author-generated CSV outputs recovered from the original `manuscript_v6/final_validation_v7` research folders in Google Drive:

| File | Content |
| --- | --- |
| `pooled_lp_full_25h.csv` | Pooled cumulative CPI response, h = 0–24, HAC SE, Holm p, and Bonferroni familywise bands |
| `country_lp_selected_horizons.csv` | 23 country coefficients at h = 0, 3, 6, 12 (92 rows); not all 25 country horizons |
| `joint_wald_tests.csv` | Four Wald equality tests for h = 0, 3, 6, 12 |
| `pooled_bootstrap_selected_horizons.csv` | Conditional block-score bootstrap results at 5 selected horizons |
| `joint_wald_bootstrap.csv` | Bootstrap inference for four country-equality tests |
| `leave_one_country_out.csv` | 92 country exclusion tests |
| `gdp_size_gdppc_interactions.csv` | Two-way fixed-effect GDP size and income moderator results |
| `gdp_size_influence_checks.csv` | GDP moderator influence and selected energy interactions |
| `region_interaction_tests.csv` | Geographic moderator tests |
| `robustness_alternative_specs.csv` | Alternative dynamic controls and study periods |
| `us_cpi_u_sensitivity.csv` | Alternative U.S. CPI-U comparison |
| `selected_main_estimates.csv` | Selected manuscript results from v7 |

The `figures/` folder contains the *unchanged original image bytes* for Figures 1–3 sourced from the v6 output folder. **The 2026 oil-price context Figure 4 is not part of this upload**, because its final provenance and exact manuscript version require a separate audit.

**Internal numerical cross-check completed:** The selected v7 pooled coefficients match the v6 pooled output for the overlapping horizons; v7 and v6 Wald test statistics agree for h = 0, 3, 6, 12. This does not replace a reproduction run from raw inputs.

**Important CPI source warning:** `data_sources.csv` reports baseline availability and identifies *candidate* LSEG RICs from an earlier provisional quality-assurance table. Those candidate codes were not marked approved or definition/date-basis verified in the original QA register; consequently, the `regression_RIC_exactly_confirmed` field is `False` throughout. Some candidates involve historical monthly standardization of quarterly-source data. **Do not cite these candidate codes as definitively used in the regressions until checked against the final panel construction code.**

**Code availability:** No original local-projection or bootstrap scripts have yet been located and validated for public release. The deposited CSVs provide numerical auditability but **not full independent re-estimation**.

## Reproducibility and limitations

The replication materials will distinguish publicly shareable research outputs from licensed source observations. Results should not be represented as independently reproduced until the corresponding data, code, software environment, and numerical checks have been deposited and verified.

## Citation

Please cite the final published article when available. A persistent repository DOI has **not yet been assigned**; no journal acceptance or publication is implied.

## Contact and contributions

For questions about this research repository, please use the GitHub Issues tab. Do not post proprietary data, passwords, or API credentials in issues or commits.
