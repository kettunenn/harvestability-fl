fed-harvest

Federated learning framework for multimodal (RGB + spectral) harvestability prediction across distributed indoor-farming sites.

🚧 Status: early scaffolding. This repository is public ahead of the code — motivation and setup below, implementation landing in stages. Watch/star if you want to follow along.

Overview

On-site indoor farms generate plant, environmental, and production data at geographically distributed sites, with heterogeneous (non-IID) conditions across locations. This project develops a federated learning framework for predicting harvestability — whether a plant or batch will meet timing, yield, and quality requirements within its harvest window — from paired RGB and calibrated spectral imagery, without centralizing raw plant imagery or operational data from individual sites.

The approach connects:

low-cost RGB plant monitoring deployed across a real-world production network,
multimodal plant-state representation (RGB + spectral ground truth),
cross-site federated learning, evaluated against site-local and centralized baselines.
Context

This work is carried out as part of an industrial PhD within the RELIANT Industrial Graduate School at Mälardalen University, in collaboration with:

Mälardalen University (academic host)
SweGreen AB — real-world indoor-farming deployment and data
Cicor Nordic Engineering AB — industrial partner

RELIANT is funded by the KK-stiftelsen (Swedish Knowledge Foundation).

What's here / roadmap

Nothing runnable yet. Planned, roughly in order:

 Data schema + synthetic/sample data for reproducibility (real SweGreen production data will not be published here — see Data below)
 Plant-state representation model (RGB → spectral-calibrated ground truth)
 Federated aggregation setup and baselines (site-local, centralized, shared FL, site-adapted FL)
 Evaluation harness and results
Data

Real operational and imagery data from SweGreen production sites is proprietary and will not be published in this repository. Sample/synthetic data for reproducing the pipeline will be added as the code lands. Access to real data is by arrangement with SweGreen.

License

To be finalized — likely Apache-2.0 for code, pending sign-off from project partners. Do not assume code here is licensed for reuse until a LICENSE file is added.
