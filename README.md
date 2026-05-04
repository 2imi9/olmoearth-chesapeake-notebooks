# OlmoEarth Chesapeake Bay Notebooks

Hands-on Jupyter notebooks for exploring monthly nutrient loading in the Chesapeake Bay watershed using the [`OlmoEarth-v1-Chesapeake-Bay-Nutrient-Loads`](https://huggingface.co/datasets/BAIGroup/OlmoEarth-v1-Chesapeake-Bay-Nutrient-Loads) dataset on Hugging Face.

**Audience:** Civil & Environmental Engineering practitioners and researchers.

## Dataset

- **Source:** [`BAIGroup/OlmoEarth-v1-Chesapeake-Bay-Nutrient-Loads`](https://huggingface.co/datasets/BAIGroup/OlmoEarth-v1-Chesapeake-Bay-Nutrient-Loads)
- **Records:** 14,200 monthly observations
- **Stations:** 121 USGS gauges across the Chesapeake watershed
- **Time:** 2014 – 2021
- **Variables:** total nitrogen (TN), total phosphorus (TP), sediment loads — plus quantile-binned classes (0–3) and flow-normalized flags per metric
- **License:** Apache-2.0

## Notebooks

| # | Notebook | Purpose |
|---|---|---|
| 01 | `01_demo.ipynb` | First-look demo: load, plot, summarize |
| 02 | `02_data_prep.ipynb` | End-to-end dataset reproduction from raw USGS sources |
| 03 | `03_tutorial_embeddings.ipynb` | OlmoEarth embedding extraction + kNN/Linear-Probe classifier (real Sentinel-2 from Planetary Computer) |
| 04 | `04_analysis.ipynb` | Cross-station analysis: persistence, sub-basin contributions, seasonality |

## Quick Start

```bash
git clone https://github.com/2imi9/olmoearth-chesapeake-notebooks.git
cd olmoearth-chesapeake-notebooks
python -m venv .venv
source .venv/bin/activate    # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook
```

Python 3.11 required.

## Citation

```bibtex
@dataset{qi2026chesapeake_nutrients,
  author    = {Qi, Ziming and BAI Group},
  title     = {OlmoEarth-v1-Chesapeake-Bay-Nutrient-Loads: Nutrient Load Reference Dataset},
  year      = {2026},
  publisher = {Hugging Face},
  url       = {https://huggingface.co/datasets/2imi9/OlmoEarth-v1-Chesapeake-Bay-Nutrient-Loads}
}
```

## Source Data Attribution

- **USGS NWIS** — [waterdata.usgs.gov](https://waterdata.usgs.gov/) (public domain)
- **Chesapeake Bay Program Data Hub** — [datahub.chesapeakebay.net](https://datahub.chesapeakebay.net/)

## Acknowledgments

This repository — notebooks, documentation, and scaffolding — was developed in collaboration with Claude Opus 4.7 (Anthropic).

## License

MIT for code in this repo · Apache-2.0 for the underlying dataset.
