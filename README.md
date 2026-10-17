# Replication Materials: Global Oil Supply News and Uneven Consumer Price Transmission

This repository is being prepared as supporting material for the manuscript:

**Global Oil Supply News and Uneven Consumer Price Transmission: Implications for Middle East Energy Risks**

**Repository status:** Initial setup. The variable dictionary and data-availability documentation have been deposited. Numerical results, figures, and analytical code have **not yet been deposited**. The repository should not yet be described as a complete replication package.

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

The file structure below distinguishes **available** documentation from **planned** files:

```text
README.md                   # Available
DATA_AVAILABILITY.md        # Available
data_dictionary.csv         # Available
data_sources.csv            # Planned
results/                    # Planned
figures/                    # Planned
code/                       # Planned
requirements.txt            # Planned
```

Where source data can lawfully be shared, the project aims to include verified analytical outputs, figure data, documented code, and sufficient instructions to reproduce the reported calculations with independently obtained licensed input data.

## Reproducibility and limitations

The replication materials will distinguish publicly shareable research outputs from licensed source observations. Results should not be represented as independently reproduced until the corresponding data, code, software environment, and numerical checks have been deposited and verified.

## Citation

Please cite the final published article when available. A persistent repository DOI has **not yet been assigned**; no journal acceptance or publication is implied.

## Contact and contributions

For questions about this research repository, please use the GitHub Issues tab. Do not post proprietary data, passwords, or API credentials in issues or commits.
