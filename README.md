# within-memory-scales

This repository contains a small example of constructing and comparing "within-memory" scales. Each item on a questionnaire can be classified by a participant as either **Remembered** (episodic) or **Known** (semantic). The provided R Markdown file demonstrates how to build separate subscales from these responses and evaluate their reliability and correlations with other variables.

## Contents

- **Toxic_example.csv** – example data from a 30‑item toxic leadership questionnaire. For every item the dataset includes the item rating and a column indicating whether the response was Remembered or Known (columns ending in `_RK`). Additional columns include liking, affective and cognitive trust, organizational citizenship behaviours (OCBI/OCBO) and commitment scores.
- **walkthrough.01.Rmd** – step‑by‑step R Markdown script showing how to:
  1. load the example data,
  2. separate items into Remember and Know sets,
  3. compute participant‑level means and frequencies,
  4. adjust reliabilities using the Spearman–Brown formula,
  5. calculate correlations with the trust and commitment measures,
  6. compare those correlations using `cocor`.

The script is a work in progress and serves as a simple illustration of the method.

## Usage

1. Open `walkthrough.01.Rmd` in RStudio (or another R environment).
2. Install the required R packages: `tidyverse`, `cocor`, `CTT` and `psych`.
3. Run the code blocks to reproduce the analysis using the example dataset.

## License

This project is released under the MIT License; see `LICENSE` for details.
