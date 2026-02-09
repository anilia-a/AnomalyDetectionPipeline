## About

This project builds a 3 layer pipeline for explaining time series novelty detection decisions:

1. **Detection** — Compares 4 novelty detectors (CNN Autoencoder, Isolation Forest, One Class SVM, Local Outlier Factor)
2. **Counterfactual Generation** — Retrieves the nearest normal training sample as a contrastive reference
3. **LLM Explanation** — Translates feature level differences into natural language explanations

The pipeline is validated across three domains: astronomical (StarlightCurves), industrial (FordA) and medical (PTB-XL).

## Datasets

Large data files are not included in this repository. Download them from the following sources:

- **StarlightCurves** — [UCR Time Series Archive](https://www.cs.ucr.edu/~eamonn/time_series_data_2018/)
- **FordA** — [UCR Time Series Archive](https://www.cs.ucr.edu/~eamonn/time_series_data_2018/)
- **PTB-XL** — [PhysioNet](https://physionet.org/content/ptb-xl/1.0.3/)

## Setup

```bash
git clone https://github.com/anilia-a/MScDissertation.git
cd MScDissertation
pip install -r requirements.txt
```
