This is a draft presentation structured to follow the outline and key points presented in the abstract, drawing heavily on the specific research context provided in the sources, particularly regarding heritage microclimate monitoring.

***

## Presentation Draft: From Sensors to Sustainability: Reliable Data Pipelines for Heritage and Infrastructure Resilience

**(Based on the Keynote Abstract: keySmarTRS2025)**

### Slide 1: Title and Introduction

**Title:** From Sensors to Sustainability: Reliable Data Pipelines for Heritage and Infrastructure Resilience

**Presenter:** [Assoc. Prof. Dr. Mohd Murtadha Mohamad]

**Affiliation:** Faculty of Computing, Universiti Teknologi Malaysia (UTM)

---

**Key Message:** The resilience of physical systems—both modern infrastructure and heritage assets—is now intrinsically linked to the **reliability of the data pipelines** that monitor them.

### Slide 2: The Core Challenge: Reliability under Stress and Uncertainty

**The Shared Fundamental Challenge:**
Modern infrastructure and heritage assets face a common challenge: maintaining **reliability under environmental stress and data uncertainty**.

*   **Environmental Stressors:** Heritage buildings, for instance, face increasing preservation challenges due to environmental factors, particularly microclimate elements like temperature, relative humidity, precipitation, and wind speed. Fluctuations in these conditions can lead to material deterioration, structural damage, and mold growth.
*   **Data Reliability Defines System Resilience:** As maintenance decisions rely increasingly on IoT sensors, remote-sensing platforms, and AI models, the reliability of the entire data pipeline (from acquisition to analytics) dictates the resilience of the physical systems being monitored.
*   **Limitations of Traditional Methods:** Traditional maintenance often relies on periodic inspections, which may fail to detect emerging issues early enough to prevent deterioration.

### Slide 3: An End-to-End Framework for Intelligent Monitoring

**Proposed Solution:** An end-to-end framework integrating heterogeneous sensors, cloud-edge analytics, and explainable machine learning.

| Component | Function / Source Detail |
| :--- | :--- |
| **Heterogeneous Sensors/Data Acquisition** | Utilizing IoT sensors and remote-sensing platforms for continuous monitoring. Modern microclimate monitoring often relies on the **Internet of Things (IoT)** paradigm to enable scalable and adaptive real-time data collection. |
| **Data Source Example** | For microclimate monitoring, data can be collected from sources like the **Copernicus Climate Data Store (ERA5 dataset)**, providing high-resolution atmospheric reanalysis data. |
| **Cloud-Edge Analytics** | Processing massive climate information, customizing models, and summarizing results into informative visualizations. |
| **Explainable Machine Learning (XAI)** | Deriving actionable insights using models that are interpretable. This helps provide a data-driven approach to prioritizing maintenance tasks. |

### Slide 4: Technical Pillars for Data Reliability

**Emphasis on Fault Tolerance and Trust:** Reliability metrics must translate computational confidence into **engineering trust**.

1.  **Fault-Tolerant Data Ingestion:** Ensuring the integrity and availability of data even when facing challenges such as missing information or concerns regarding data source dependability. The process involves collecting, cleaning (removing duplicates/inconsistencies), and transforming raw data to ensure its quality and reliability for subsequent analysis.
2.  **Adaptive Model Retraining (Mitigating Sensor Drift):** Models must remain relevant over time. This involves monitoring the model's performance and continuously retraining to mitigate issues like sensor drift.
3.  **Reliability Metrics and Performance Evaluation:** Using metrics to ensure the models are accurate and reliable. For classification tasks, key metrics include **Accuracy, Precision, Recall, and F1-score**.

### Slide 5: Case Study: Heritage Microclimate Monitoring

**Application in Heritage Preservation:** Case studies in heritage microclimate monitoring illustrate the framework's effectiveness.

**Project Focus:** Predicting maintenance priorities for heritage buildings in Johor Bahru, Malaysia, based on microclimate conditions.

**Key Microclimate Parameters Used:** Temperature, relative humidity, wind speed, and precipitation.

**Model Development:** Six machine learning techniques were evaluated for predicting maintenance priority ratings: XGBoost, decision tree (DT), logistic regression, recurrent neural network (RNN), support vector machine (SVM), and linear regression.

**Results Highlight (Model Performance):**
*   The **XGBoost model** demonstrated superior performance.
*   XGBoost achieved the highest **testing accuracy of 88%** and an **F1-score of 0.88**.
*   The Decision Tree model achieved the lowest MAE of 0.75, MSE of 1.00, and RMSE of 1.00 in one evaluation, but overall XGBoost proved the most effective and reliable.
*   Deep learning architectures like RNN performed poorly, likely due to the small dataset size inherent to heritage studies.

### Slide 6: Actionable Insights through Explainability (XAI)

**Interpretability is Key:** Interpretability allows non-technical stakeholders to rely on and utilize the model’s predictions in practical heritage conservation planning.

*   The framework emphasizes **interpretable models and rule-based scoring**.
*   **Rule Extraction from XGBoost:** The study included the extraction of rules from the best-performing XGBoost model to support practical decision-making.
*   **Example Extracted Rule:** If the wind speed is low (less than 3.5 m/s) and the temperature is also low (less than 28.2°C), the building is more likely to be in good condition.
*   **Decision Support:** Predictive results can be visualized in a user-friendly Power BI dashboard for effective monitoring and decision making. This facilitates the shift to **proactive maintenance**, which reduces long-term repair costs and extends the lifespan of heritage buildings.

### Slide 7: Conclusion and Design Guidelines

**Core Principles for Intelligent and Resilient Technologies:**

The framework concludes with design guidelines for AI-enabled monitoring systems that are:

1.  **Verifiable:** Predictions must be validated against real-world data and clear metrics (e.g., Accuracy, F1-score).
2.  **Maintainable:** The system must incorporate adaptive model retraining to handle evolving environmental conditions and data drift.
3.  **Sustainable:** Predictive modeling supports evidence-based conservation policies, enhances resource allocation, and leads to timely interventions, contributing to the **sustainable preservation** of cultural heritage sites. Proactive decisions reduce the need for costly and extensive repairs, increasing economic sustainability.

**Final Thought:** By linking robust data pipelines, reliable AI, and actionable rules, we can drive the future with intelligent and resilient technologies.

![System Diagram](images/NotebookLM_Mind_Map.png)
