# EcoDriveAI+ 

##  Problem Statement

EVs are more energy-efficient than conventional vehicles, but **energy consumption still varies significantly with driving behaviour, traffic, speed, acceleration and environmental conditions**. As EV adoption grows, improving energy efficiency becomes increasingly important. The IEA projects global EV electricity demand to exceed **1,500 TWh by 2035** under its Current Policies Scenario.

The problem addressed by this project is:

> **How can AI use EV telemetry to predict energy consumption, identify inefficient driving behaviour, and provide actionable recommendations to reduce energy waste?**

---

## What I Built

**EcoDriveAI+** is an end-to-end AI system that transforms raw EV telemetry into **energy predictions, driving-behaviour insights and actionable eco-driving recommendations.**

### Dataset Used

* **EV Energy Consumption Dataset** — 5,000 records used for energy-consumption modelling.
* **Tesla Model 3 Telemetry Dataset** — 23,135 cleaned telemetry records used for real-world behavioural and vehicle analysis.

### What the code implements

**Data Engineering → Feature Engineering → ML Prediction → Behaviour Clustering → Explainable AI → EcoDrive Score → Counterfactual Simulation → Recommendations → Interactive Dashboard**

---

## Key Results

| Metric                  |                        Result |
| ----------------------- | ----------------------------: |
| EV training records     |                     **5,000** |
| Tesla telemetry records |                    **23,135** |
| Model R²                |                     **0.941** |
| Average EcoDrive Score  |                **92.1 / 100** |
| ML models compared      |                         **5** |
| Behaviour analysis      |        **K-Means clustering** |
| Dashboard               | **Interactive Dash + Plotly** |

The final pipeline compares 5 regression approaches rather than assuming one model is optimal, and evaluates predictions using MAE, RMSE, and R².

---

## What I Improved

The project was developed beyond a basic EV energy-prediction model.

### From basic prediction → complete AI decision system

* Expanded the modelling pipeline from **6 basic driving features** to a broader feature set covering **speed, acceleration, jerk, variability, traffic stress, battery, weather, vehicle and road characteristics**.
* Added **Jerk and harsh-driving detection** to capture sudden driving behaviour.
* Replaced arbitrary behaviour classification with **data-driven K-Means clustering + silhouette analysis**.
* Added an **EcoDrive Score (0–100)** instead of presenting raw telemetry alone.
* Added **counterfactual simulation** to estimate potential energy savings under smoother driving.
* Added **explainable AI / feature importance / SHAP analysis** to understand what drives predictions.
* Added **energy-based route comparison** rather than considering only distance or travel time.
* Added an **interactive dashboard** for non-technical users.

### Unique Contribution

Most EV prediction projects stop at:

**“Predict energy consumption.”**

EcoDriveAI+ goes further:

**Predict → Explain → Detect Behaviour → Score → Recommend → Simulate Savings → Support Decisions**

This makes the project a prototype AI decision-support system for sustainable EV and fleet management, not just a machine-learning model.

---

##  Business Impact

EcoDriveAI+ could help EV fleet operators:

* Reduce unnecessary energy consumption
* Identify inefficient driving patterns
* Provide personalized driver coaching
* Compare vehicle and route efficiency
* Reduce charging and operating costs
* Improve effective driving range
* Monitor fleet energy performance

For a fleet, even a small efficiency improvement repeated across **thousands of kilometres and hundreds of vehicles** can translate into meaningful energy and cost savings.

The approach is also aligned with the broader importance of behavioural energy efficiency: the IEA identifies **eco-driving and avoiding sudden acceleration/stops** as relevant transport-efficiency measures.

---

## Social & Environmental Impact

The project aims to reduce **energy waste per kilometre**, encourage smoother driving and support more efficient use of growing EV fleets.

The environmental impact is not claimed as a measured reduction from this prototype; the **energy savings are model-based estimates** that would require real-world driver testing for validation.

---

## Conclusion

**EcoDriveAI+ demonstrates how AI can move EV analytics from passive monitoring to actionable optimization.**

Instead of simply asking,*“How much energy did the EV consume?”*. The system asks,**“Why did it consume that energy, how did the driver behave, what can be improved, and what could happen if driving behaviour changes?”**

The result is an end-to-end prototype combining **machine learning, behavioural analytics, explainable AI and sustainability-focused decision support** for future EV and fleet-management applications.
