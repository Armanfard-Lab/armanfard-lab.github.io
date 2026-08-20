---
title: "iSMART Lab - Datasets"
layout: textlay
excerpt: "Datasets"
sitemap: true
permalink: /datasets/
---

## Datasets

### <span id="enginead">EngineAD</span>

EngineAD is a real-world vehicle engine anomaly detection dataset designed for safety-critical transportation applications.

- Collected from a fleet of **25 commercial vehicles** over **6 months**.
- Includes high-resolution telemetry sampled at approximately **1-second intervals** from engine-related sensors.
- Covers **13 raw engine signals** (e.g., pressure, temperature, fuel-rate, rotational-speed related channels).
- Includes expert annotations distinguishing normal operation from early signs of incipient faults.
- Provides processed segment-level data commonly used for benchmarking (including principal-component-based representations).

The EngineAD dataset is now publicly available — no access request is required. To download it, please visit the dataset page below.

**Dataset page:** [BorealisData - EngineAD (DOI:10.5683/SP3/TX13P1)](https://borealisdata.ca/dataset.xhtml?persistentId=doi:10.5683/SP3/TX13P1)

**Related papers:**
- [EngineAD: A Real-World Vehicle Engine Anomaly Detection Dataset (AAAI ASTAD 2026)](https://arxiv.org/abs/2603.25955)
- [Multivariate Time-Series Anomaly Detection with Temporal Self-supervision and Graphs (ECML PKDD 2023)](https://doi.org/10.1007/978-3-031-43430-3_15)

**Citation policy:** If you use EngineAD, please cite both papers below.

```bibtex
@inproceedings{hojjati2026enginead,
  title={EngineAD: A Real-World Vehicle Engine Anomaly Detection
    Dataset},
  author={Hojjati, Hadi and Roth, Christopher and Woods, Rory and
    Sills, Ken and Armanfard, Narges},
  editor={Armanfard, Narges and Hojjati, Hadi and Ho, Thi Kieu
    Khanh},
  booktitle={Automated Spatial and Temporal Anomaly Detection:
    Third International Workshop, ASTAD@AAAI 2026, Held in
    Conjunction with AAAI 2026, Singapore, January 26, 2026,
    Proceedings},
  series={Communications in Computer and Information Science},
  year={2026},
  publisher={Springer Singapore},
  address={Singapore}
}
```

```bibtex
@inproceedings{hojjati2023multivariate,
  title={Multivariate Time-Series Anomaly Detection with Temporal
    Self-supervision and Graphs: Application to Vehicle Failure
    Prediction},
  author={Hojjati, Hadi and Sadeghi, Mohammadreza and Armanfard,
    Narges},
  booktitle={Machine Learning and Knowledge Discovery in
    Databases: Applied Data Science and Demo Track (ECML PKDD)},
  series={Lecture Notes in Computer Science},
  volume={14175},
  pages={239--254},
  year={2023},
  publisher={Springer},
  doi={10.1007/978-3-031-43430-3_15}
}
```

### <span id="multitab">MultiTab — Synthetic Multitask Data</span>

Generate synthetic multitask regression datasets with controllable task correlations, polynomial complexity, and noise levels.

**Generator:** [Open the MultiTab generator →](/multitab-generator/)

**Related paper:**
- [MultiTab: A Scalable Foundation for Multitask Learning on Tabular Data (AAAI 2026)](https://arxiv.org/abs/2511.09970)

**Citation policy:** If you use MultiTab or the synthetic generator for experiments, please cite the paper below.

```bibtex
@inproceedings{sinodinos2026multitab,
  title={MultiTab: A Scalable Foundation for Multitask Learning on Tabular Data},
  author={Sinodinos, Dimitrios and Wei, Jack Yi and Armanfard, Narges},
  booktitle={Proceedings of the AAAI Conference on Artificial Intelligence},
  volume={40},
  number={30},
  pages={25499--25507},
  year={2026}
}
```

### Upcoming datasets

#### CARLA-Collide

*Description to be added.*

**Link:** [TBD](#)

#### Real-Collide

*Description to be added.*

**Link:** [TBD](#)
