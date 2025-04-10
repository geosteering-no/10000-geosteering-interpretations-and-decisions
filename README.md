# 10,000 Interpretations and Decisions from the Geosteering World Cup 2021

This dataset supports the article:  
**“Analyzing Expert Decision-Making in Geosteering: Statistical Insights from a Large-Scale Controlled Experiment”**  
Y. Cheraghi, S. Alyaev, R.B. Bratvold, A. Hong, I. Kuvaev, S. Clark, A. Zhuravlev  
[Applied Computing and Geosciences, 2025](https://doi.org/10.1016/j.acags.2025.100237)

## Overview

This dataset contains around 10,000 time-stamped geosteering interpretations and directional drilling decisions collected during the Geosteering World Cup 2021—a large-scale, controlled experiment involving 349 expert participants. Each participant interacted with a simulated geosteering environment using real-time log data and SBS (Stratigraphy-Based Steering) techniques to steer wells through complex subsurface formations.

The dataset includes sequential interpretation snapshots, well trajectories, and evaluation metrics, making it well-suited for studies in decision-making under uncertainty, human-AI interaction, and subsurface modeling. Two distinct drilling scenarios (conventional and unconventional) are featured, with all participants using the same baseline model and tools, enabling direct comparison of decision strategies and outcomes.

## Directory Structure
```
LICENSE.txt                  # CC-BY 4.0 license text
README.md                    # Dataset documentation
round1.zip                   # Geosteering data for Round 1 (unconventional scenario)
├── interpretations_csv/     # Step-by-step interpretation CSVs for each participant
└── json/                    # JSON files with full player data (interpretations + trajectories)
round2.zip                   # Geosteering data for Round 2 (conventional scenario)
├── interpretations_csv/     # Step-by-step interpretation CSVs for each participant
└── json/                    # JSON files with full player data (interpretations + trajectories)
schema.json                  # JSON schema for player data format
schema_answer.json           # JSON schema for answer (ground truth) format
time-lapse-example/          # Example images for a time-lapse of a single participant
```

## Usage
Extract `round1.zip` or `round2.zip` and read the `json/` files to access full player interpretation logs and final trajectories.
 - The `schema.json` and `schema_answer.json` files provide the structure of the JSON format for each time lapse and the answer (ground truth) format, respectively.
 - The `interpretations_csv/` directory contains CSV files with interpolated interpretations for each participant for each step, which can be easier to work with. They are linked in the JSON files.

## Data Collection & Processing

Around 10,000 snapshots were recorded through an online system, consisting of interpretations of log data for each participant's well and corresponding decisions, every 2 minutes. These snapshots form a comprehensive database that is useful and valuable to provide insights into the decision-making process of the geosteerers and learning for improving geosteering decision-making. The dataset utilized in this study is openly accessible and published alongside the paper.



## License
This dataset is licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). You are free to share and adapt the material for any purpose, even commercially, as long as you give appropriate credit to the original authors and indicate if changes were made.

### Cite as

**This article**:  
Cheraghi, Y., Alyaev, S., Bratvold, R. B., Hong, A., Kuvaev, I., Clark, S., & Zhuravlev, A. (2025).  
*Analyzing Expert Decision-Making in Geosteering: Statistical Insights from a Large-Scale Controlled Experiment*.  
**Applied Computing and Geosciences**. https://doi.org/10.1016/j.acags.2025.100237

**The dataset**:  
Alyaev, S., Cheraghi, Y., Kuvaev, I., Clark, S., & Zhuravlev, A. (2025).  
*Supporting Data for Over 10,000 Directional Drilling Decisions from the Geosteering World Cup 2021* [Dataset].  
**Zenodo**. https://doi.org/10.5281/zenodo.XXXXXXX

```bibtex
@article{Cheraghi2025Geosteering,
  title     = {Analyzing Expert Decision-Making in Geosteering: Statistical Insights from a Large-Scale Controlled Experiment},
  author    = {Yasaman Cheraghi and Sergey Alyaev and Reidar B. Bratvold and Aojie Hong and Igor Kuvaev and Stephen Clark and Andrei Zhuravlev},
  journal   = {Applied Computing and Geosciences},
  year      = {2025},
  doi       = {10.1016/j.acags.2025.100237},
  note      = {In press},
  publisher = {Elsevier},
  url       = {https://doi.org/10.1016/j.acags.2025.100237}
}

@misc{Alyaev2025Dataset,
  author       = {Alyaev, Sergey and Cheraghi, Yasaman and Kuvaev, Igor and Clark, Stephen and Zhuravlev, Andrei},
  title        = {Supporting Data for Over 10,000 Directional Drilling Decisions from the Geosteering World Cup 2021},
  year         = {2025},
  publisher    = {Zenodo},
  doi          = {10.5281/zenodo.XXXXXXX},
  url          = {https://doi.org/10.5281/zenodo.XXXXXXX},
  note         = {Version 1.0}
}
```

### Related dataset:

```bibtex
@misc{geology-forecast-challenge-open,
    author = {Sergey Alyaev and Nello Blaser and Anton Fedorov and Igor Kuvaev},
    title = {Geology Forecast Challenge},
    year = {2025},
    howpublished = {\url{https://kaggle.com/competitions/geology-forecast-challenge-open}},
    note = {Kaggle}
}
```

### Related articles:

There are two older articles that use the data from the Geosteering World Cup 2021. The first one is a conference paper with the intial analysis of the results and the second one is a JPT article that discusses the results of the competitio in the context of geosteering industry.

```bibtex
@proceedings{10.15530/urtec-2022-3722510,
    author = {Cheraghi, Yasaman and Alyaev, Sergey and Hong, Aojie and Kuvaev, Igor and Clark, Stephen and Zhuravlev, Andrei and Bratvold, Reidar Brumer},
    title = {What Can We Learn After 10,000 Geosteering Decisions?},
    volume = {Day 2 Tue, June 21, 2022},
    series = {SPE/AAPG/SEG Unconventional Resources Technology Conference},
    pages = {D021S022R002},
    year = {2022},
    month = {06},
    doi = {10.15530/urtec-2022-3722510},
    url = {https://doi.org/10.15530/urtec-2022-3722510},
    eprint = {https://onepetro.org/URTECONF/proceedings-pdf/22URTC/2-22URTC/D021S022R002/2802308/urtec-3722510-ms.pdf},
}
@article{10.2118/1222-0024-JPT,
    author = {Rassenfoss, Stephen},
    title = {A Study Suggests Geosteers Often Are Missing the Target},
    journal = {Journal of Petroleum Technology},
    volume = {74},
    number = {12},
    pages = {24-29},
    year = {2022},
    month = {12},
    issn = {0149-2136},
    doi = {10.2118/1222-0024-JPT},
    url = {https://doi.org/10.2118/1222-0024-JPT},
    eprint = {https://onepetro.org/JPT/article-pdf/74/12/24/3065565/spe-1222-0024-jpt.pdf},
}
```

