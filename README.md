# Detecting-Concept-Drift
Short-form video platforms evolve rapidly, making static recommendation models obsolete.
This project builds an adaptive ML framework to classify video trend trajectories and detect concept drift over time, ensuring sustained relevance in fast-moving content ecosystems.

The system combines momentum-based trend prediction with rolling validation and adaptive learning, simulating a production environment where user behavior continuously shifts.

<p align="center">
  <img src="CD1.png" width="850">
</p
<p align="center">
  <img src="CD2"  width="850">
</p

### [Data Preprocessing](Machine%20Learning%20Project%20Data%20Preprocessing.ipynb)

- Data Source - https://www.kaggle.com/datasets/tarekmasryo/youtube-shorts-and-tiktok-trends-2025
- Builds a unified, multi-platform dataset of 50K+ videos
- Cleans, encodes, and normalizes engagement metrics across platforms and regions
- Engineers high-signal momentum features (relative performance, velocity, growth rates)
- Produces a leakage-free, modeling-ready feature set

### [Exploratory Data Analysis](EDA_DriftDetection.ipynb)

- Explores trend dynamics and extreme class imbalance
- Reveals boom-or-bust behavior in short-form video engagement
- Analyzes how platform, category, language, and timing affect virality
- Establishes structural motivation for adaptive modeling

### [Detecting Concept Drift via Statistical Methods](Statistical_Methods.ipynb)

- Applies Population Stability Index (PSI) to detect data and target drift
- Quantifies distributional shifts across monthly windows
- Provides statistical evidence of concept drift before model failure

### [Evaluating Baseline Classifiers](AML_Project_Baseline_Models.ipynb)

- Trains baseline classifiers (Logistic Regression, Random Forest)
- Evaluates performance under severe imbalance
- Demonstrates the limitations of static models in dynamic environments

### [Evaluating Ensembles and Incremental Learners](AML_Project_Concept_Drift_Models.ipynb)

- Implements adaptive and streaming models for evolving data
- Uses rolling, month-by-month validation to simulate production
- Evaluates ensemble and incremental learners
- Shows sustained performance gains under concept drift
