# Netflix Executive Dashboard

An executive dashboard and analysis for Netflix management, built in a 2-week sprint and managed on a GitHub Projects Kanban board.

## Business question
If you were presenting to Netflix executives, which KPIs would you monitor?

## Sprint goal
By the end of the 2-week sprint, deliver a working executive dashboard prototype built on the 500-record viewing and ratings dataset. It shows 5 agreed KPIs on one page, with filters for membership, genre and country. The KPI calculations are validated against the raw data and the prototype has been reviewed by a stakeholder.

The full sprint goal is in [Sprint Goal.docx](Sprint%20Goal.docx).

## KPIs monitored
| KPI | Definition | Why it matters |
|---|---|---|
| Total views | Number of viewings | Measures overall usage |
| Unique viewers | Distinct `User_Id` values | Measures audience reach |
| Average rating | Mean of `Ratings` (1 to 5) | Tracks content satisfaction |
| Hours watched | Views × movie duration ÷ 60 | Measures engagement |
| Rated 4 stars or more | Share of ratings of 4 or 5 | Shows how many viewers are satisfied |

## Repository structure
```
.
├── Netflix_Project_Analysis/
│   ├── Netflix Executive Dashboard.html
│   ├── Netflix_Cleaned_Dataset.csv
│   ├── Netflix_Dataset.csv
│   ├── Netflix_Project.html
│   ├── Netflix_Project.ipynb
│   └── Screenshots_of_Suceessfull_Run.png
├── Project Plan.pdf
├── README.md
├── RETROSPECTIVE.md
└── Sprint Goal.pdf
```

| File | Description |
|---|---|
| [Netflix Executive Dashboard.html](Netflix_Project_Analysis/Netflix%20Executive%20Dashboard.html) | The executive dashboard. Open it in any web browser. Use the filters to explore the KPIs. |
| [Netflix_Dataset.csv](Netflix_Project_Analysis/Netflix_Dataset.csv) | The original dataset (raw data, one row per viewing). |
| [Netflix_Cleaned_Dataset.csv](Netflix_Project_Analysis/Netflix_Cleaned_Dataset.csv) | The dataset after cleaning and validation, used for the dashboard KPIs. |
| [Netflix_Project.ipynb](Netflix_Project_Analysis/Netflix_Project.ipynb) | Jupyter notebook with the data cleaning and analysis. |
| [Netflix_Project.html](Netflix_Project_Analysis/Netflix_Project.html) | HTML export of the notebook, readable without running any code. |
| [Screenshots_of_Suceessfull_Run.png](Netflix_Project_Analysis/Screenshots_of_Suceessfull_Run.png) | Screenshot showing the notebook running successfully. |
| [Project Plan.docx](Project%20Plan.pdf) | Project plan: tasks, owners, estimates and risks. |
| [Sprint Goal.docx](Sprint%20Goal.pdf) | The sprint goal and how it is measured. |
| [RETROSPECTIVE.md](RETROSPECTIVE.md) | Sprint retrospective: what went well, what did not and the next actions. |

## Dataset
- One row per viewing, 500 rows.
- Columns: `Movie_id`, `Movie_Title`, `Genre`, `Year_of_release`, `Movie_duration` (minutes), `Watched_Country`, `Watched_date`, `User_Id`, `Ratings`, `Average_Ratings`, `Membership` (Premium, Standard or Basic).
- The data is **synthetic**, created for a class project. It is not real Netflix data.

## How to use
1. **See the dashboard:** download `Netflix Executive Dashboard.html` and open it in a web browser.
2. **See the analysis:** open `Netflix_Project.html` in a browser, or run `Netflix_Project.ipynb` in Jupyter Notebook or Google Colab.
3. **Reuse the data:** load `Netflix_Cleaned_Dataset.csv` into Excel, Power BI, Tableau or Python (pandas).

## Project management
- **Kanban board:** [(https://github.com/users/YaqootRuby/projects/1)]
- **Columns:** Backlog, Ready, In Progress, In Review, Done
- **Rules:** maximum 2 cards per person in progress. A card is Done only after someone else has reviewed it.
- **Cards:** 12 sprint tasks with an owner and estimate, 3 backlog items and 2 risk cards.

## Team and roles
| Name | Role |
|---|---|
| Yaqoot Bibi | Product Owner |
| Mehejabin Hossain Jitu | Scrum Master |
| Mehejabin Hossain Jitu, Yaqoot Bibi | Data Engineer |
| Mehejabin Hossain Jitu, Yaqoot Bibi | Data Analyst |
| Yaqoot Bibi, Mehejabin Hossain Jitu | Dashboard Developer |

## Risks and mitigation
| Risk | Mitigation |
|---|---|
| **Inconsistent or poor-quality data**: KPIs do not match the source, or definitions differ between team members | Written KPI definitions, automated data-quality checks and analyst validation of every KPI against the raw data |
| **Dashboard overload and low executive adoption**: too many metrics or a cluttered design | Limit the front page to 5 KPIs, review the wireframe with the Product Owner before building and hold a short stakeholder walkthrough |

## Retrospective
See [RETROSPECTIVE.md](RETROSPECTIVE.md) for the sprint review, lessons learned and action items.

## Limitations and next steps
- The dataset has views and ratings only, so financial KPIs such as revenue, churn and cost per viewing hour are not covered.
- Next sprint: genre drill-down, mobile view and automated daily data refresh.
