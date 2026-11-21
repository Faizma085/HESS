# Global Wet–Dry Regime Transitions

**Companion analysis code for the manuscript:**  
*Land-Surface Sensitivity and Climate Variability Shape Global Wet-Dry Regime Transitions*  *The title is revised* 
**Manuscript id:** egusphere-2026-4696  
## Research scope

The analysis describes spatial changes in the **direction of modeled terrestrial water storage-state trends**, approximated historically from TerraClimate soil water and snow water equivalent (SWE). Historical trend signs are assessed for **1979–2000** and **2001–2023**, and a **30-model CMIP6** workflow compares recent historical and projected trends under **SSP2-4.5** and **SSP5-8.5**.

The historical classes have the following descriptive definitions:

| Class | 1979–2000 storage slope | 2001–2023 storage slope |
|---|---|---|
| **DD** | Negative | Negative |
| **WW** | Positive | Positive |
| **WD** | Positive | Negative |
| **DW** | Negative | Positive |

**Important:** DD, WW, WD and DW refer here to combinations of **fitted trend signs**, not absolute wet/dry climate categories, and not automatically to statistically significant slopes. Separate tests examine uncertainty and slope changes. All gridded fractions must use an explicitly defined common valid/ice-free land mask and terrestrial cell-area weights.

The historical customized standardized water-balance residual, referred to in some scripts as **SPEI-SR**, is calculated from \(P - AET - Q\). It is a **storage-change/residual diagnostic**, not a direct storage-state series. Consequently, residual-based results are placed in supporting/supplementary workflows rather than substituted for the direct soil+SWE primary interpretation.

# Installation and checks

Python 3.10 or later is recommended. The dependency list is inferred from code imports and is **not a tested lockfile**.

```bash
python -m venv .venv
# Linux/macOS:
source .venv/bin/activate
# Windows PowerShell: .venv\Scripts\Activate.ps1

python -m pip install --upgrade pip
python -m pip install -r requirements.txt

```

## How to cite

If citing the analysis, cite the associated HESS/EGUsphere manuscript. The manuscript identifier is **egusphere-2026-4696**. **Publication DOI, final author list, journal citation and repository release DOI must be added after verification**; no final publication information is asserted here.

## Repository use and licensing

The original source bundle did not supply an explicit software license. **No open-source reuse license is implied by posting the files to GitHub.** The repository maintainer should choose and add a `LICENSE` file only after confirming authorship, permissions, and applicable data/product terms. This README does not grant third-party rights in datasets or external materials.

## Reporting issues

When reporting a replication discrepancy, identify the script path, input product and version, expected output, actual output, relevant time window, model/member selection, coordinate and unit handling, and the applicable land mask/area denominator. Include a minimal traceback or summary table where possible, without disclosing credentials or restricted data.
