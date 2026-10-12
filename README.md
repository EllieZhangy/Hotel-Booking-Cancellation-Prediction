# Hotel Booking Cancellation Prediction

> **Archived learning project (2023).** This repository remains public as part of my applied data-science foundations. For current AI product and research work, see the selected projects at the bottom of this page.

`EDA` · `Classification` · `XGBoost` · `Clustering` · `Time Series` · `Business Analytics`

This project combines exploratory analysis, cancellation prediction, customer segmentation, and time-based demand analysis to study hotel booking behavior. The central modeling task is to identify reservations at higher risk of cancellation while preserving enough recall to support proactive operational planning.

## Project scope

| Analysis track | Methods |
| --- | --- |
| **Exploratory analysis** | Missing-value review, distributions, relationships, and business-oriented visualizations |
| **Class imbalance** | Upsampling and SMOTE |
| **Cancellation prediction** | Logistic regression, decision tree, random forest, XGBoost, and other candidate models |
| **Model validation** | K-fold cross-validation with emphasis on recall |
| **Customer segmentation** | K-Means and DBSCAN |
| **Demand patterns** | Time-series exploration of booking and cancellation behavior |

## Data

The project uses the public **Hotel Booking Demand** dataset described by Nuno António, Ana de Almeida, and Luís Nunes in *Data in Brief* (2019).

## Classification result

The model comparison emphasizes **recall**, because missing a likely cancellation can be operationally costly. XGBoost was selected as the final candidate in the original analysis.

<p align="center">
  <img width="1050" alt="Hotel cancellation model performance comparison" src="https://github.com/EllieZhangy/Hotel-Booking-Cancellation-Prediction/assets/133906690/aa0e02ef-7e26-4513-b873-8e363616a23d" />
</p>

Features highlighted in the original analysis include:

- Whether a parking space was required.
- Whether the guest had previously canceled.
- Market-segment category.

These relationships are descriptive within this dataset and should not be interpreted as causal conclusions.

## Customer segmentation

The clustering analysis produced four interpretable groups in the project narrative:

1. **Business travelers** — stronger preference for city hotels.
2. **Self-driving guests** — more likely to require parking.
3. **Group travelers** — larger party-oriented bookings.
4. **Loyal guests** — more repeat-visitor behavior.

<p align="center">
  <img width="780" alt="Geographic distribution of hotel customer segments" src="https://github.com/EllieZhangy/Hotel-Booking-Cancellation-Prediction/assets/133906690/f5995b04-c715-4f51-bb54-ecbf5929292c" />
</p>

## Repository guide

- `Code.ipynb` contains the main analysis and modeling workflow.
- `Presentation.pdf` contains the project summary and visual results.

Because this is an older coursework project, package versions and notebook runtimes may require updates before reproduction.

## Limitations

- Cancellation behavior varies by property, geography, channel, and time period; results may not generalize beyond the source data.
- SMOTE and upsampling should be applied inside the training folds to avoid leakage.
- Segment labels are interpretive summaries, not verified customer identities.
- A production system would require probability calibration, cost-sensitive thresholds, monitoring, drift checks, and review of operational consequences.
- Predictions should support—not automatically replace—human revenue-management and guest-service decisions.

## Selected work

- [AI Driving School](https://elliezhangy.github.io/ai-driving-school/) — a voice- and text-controlled Chinese parking game.
- [Daily Mood Screen](https://github.com/EllieZhangy/Daily-Mood-Screen) — a personalized macOS wallpaper pipeline using weather, photos, and mood.
- [Memory Studio](https://github.com/EllieZhangy/my-ai-poster-skills) — a photo-to-poster web app with reusable visual styles.
- [Radiology Impression Prediction](https://github.com/EllieZhangy/LLM-Based-Impression-Prediction-from-Radiology-Reports) — an LLM research project for radiology report impression generation.
