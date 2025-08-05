# student-success-analytics-jcu

### Data Disclaimer
This project was developed using synthetic data designed to simulate real-world scenarios. No actual student or university records were used at any stage.

### Objectives

1. **Flag students at high risk of underperforming** based on academic engagement and early indicators.
2. **Profile students by risk level** using attendance, assessment score, and academic support usage.
3. **Build dashboards** to support quick, evidence-based decision-making for student success teams.
4. **Lay a scalable foundation** for predictive modeling and automation when real data becomes available.

### Tools and Technologies

- **Python** (in Azure Machine Learning Studio Notebooks)
- **Power BI**
- **Excel** (for dummy dataset structure and simulation)

### Dataset

- A dummy dataset simulating real student data was used.
- Fields match the real dataset structure (e.g., `Student_ID`, `Assessment Score`, `Attendance`, etc.).
- Columns like `Course Group` and `Risk Assessment` were added during the analysis.
- Data cleaning and preprocessing were done programmatically in Python using Azure ML Studio.

### Data Cleaning and Preparation

Steps taken:
- Converted columns with percentage strings to numeric format.
- Handled missing and ambiguous values (`NA`, `?`, etc.).
- Merged data fields where necessary.
- Added derived features such as risk level categorization (High, Medium, Low).
- Ensured all values were in correct types/formats for Power BI integration.

### Visualizations in Power BI

Key interactive dashboards built:
- **Risk Flagging**: Visual flags by week (e.g., Week3, Week5, Week10).
- **Student Profiling**: View students by cohort, course group, and support usage.
- **Drill-down Filters**: Course, subject, term, and risk group filters for customized views.
- **Dynamic Metrics**: Number of students flagged, risk trends by group, GPA vs. attendance plots.

### Outcomes and Impact

- Enabled early identification of students at academic risk.
- Created a reusable and scalable risk flagging logic for real-time reporting.
- Reduced manual effort by integrating Power BI with processed student datasets.
- Improved transparency and communication between academic and support teams.
- Built a process-ready template that can be quickly adapted to real data once available.

### Future Scope & Recommendations

- Integrate this system with **real-time data pipelines** from internal databases (e.g., LearnJCU).
- Incorporate **Retention column** from the real data to build predictive models.
- Use **logistic regression or classification trees** to predict student attrition.
- Automate periodic updates and alerts using Power BI and Azure ML.
- Enhance student engagement profiling with survey or behavioral data.

### Repository Structure
```text
student-success-analytics-jcu/
│
├── notebooks/             # student_data.ipynb (Azure ML Studio)
├── PowerBI/               # Power BI dashboard files and user manuals
├── Presentations/         # Presentaion Files
├── License
└── README.md
```
### Getting Started

### Prerequisites
Python 3.8+
pip or conda
(Optional) Azure account for cloud deployment
(Optional) Power BI Desktop for dashboard visualization

### Setup
Clone the repository:

bash
git clone https://github.com/galwa506/student-success-analytics-jcu.git
cd student-success-analytics-jcu
Install dependencies:

bash
pip install -r requirements.txt
Explore the notebooks:

Open the notebooks/ folder in JupyterLab or Jupyter Notebook.

Data Preparation:

Place your de-identified or mock student data in the data/ folder, following the required schema.

Power BI Dashboards:

Open Power BI Desktop and load .pbix files from dashboards/.

Connect to processed data exports to visualize outcomes and risk profiles.

### Key Technologies
Python (pandas, numpy, scikit-learn, xgboost, etc.)

Azure ML for scalable cloud model serving

Power BI for business intelligence and dashboarding

Jupyter for interactive data analysis

### Use Cases
Academic Advisors: Identify at-risk students early for targeted intervention.

Administrators: Monitor retention trends and forecast cohorts’ academic outcomes.

Data Science Teams: Reuse and adapt reproducible pipelines for institutional research.

### Power BI Dashboards:

Open Power BI Desktop and load .pbix files from dashboards/.

Connect to processed data exports to visualize outcomes and risk profiles.

### Key Technologies
Python (pandas, numpy, scikit-learn, xgboost, etc.)

Azure ML for scalable cloud model serving

Power BI for business intelligence and dashboarding

Jupyter for interactive data analysis

### Contributing
Contributions, suggestions, and improvements are welcome! Please open an issue or submit a pull request.

### License
This project is for academic and demonstration purposes. For details, see the LICENSE file.

### Acknowledgements
Developed at James Cook University, Australia.

For questions or collaborations, please contact the repository owner via GitHub Issues.

