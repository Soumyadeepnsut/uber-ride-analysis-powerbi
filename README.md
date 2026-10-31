# Uber Ride Analysis | Power BI Dashboard

An interactive Power BI portfolio project exploring ride-booking performance, revenue, vehicle mix, customer behavior, and location-level demand. The report is organized into six pages: **Home, Overview, Vehicle, Revenue, Customer, and Location**.

> **Project type:** Data analytics and business intelligence  
> **Primary tool:** Microsoft Power BI  
> **Techniques:** KPI design, data modeling, DAX measures, time-series analysis, segmentation, and interactive report navigation

## Business problem

Ride-hailing operations generate data across bookings, revenue, vehicle types, customers, payments, and pickup/drop-off locations. This dashboard brings those views together to help stakeholders investigate:

- Where bookings and revenue are being lost.
- Which vehicle categories contribute most to revenue and completed rides.
- How payment methods and customers contribute to revenue.
- What cancellation patterns may signal customer or operational risk.
- Which locations and time slots experience greater demand.

## Dashboard pages

| Page | What it covers | Business questions |
|---|---|---|
| **Home** | Project introduction and page navigation | How can a user navigate the report? |
| **Overview** | Bookings, lost bookings, revenue, distance, average distance, monthly/quarterly trends, vehicle revenue, ratings and location highlights | What is the overall operating picture? |
| **Vehicle** | Vehicle-level bookings, revenue, revenue contribution, completion/incomplete rates and monthly completed-booking trends | Which vehicle types perform best? |
| **Revenue** | Monthly/quarterly revenue, month-over-month change, revenue by vehicle, customer and payment method, lost revenue and revenue per kilometre | Where is revenue generated or at risk? |
| **Customer** | First-time, return and regular customer segments, cancellation metrics, customer-level detail and payment preferences | What customer behaviors may affect retention and revenue? |
| **Location** | Distance by vehicle and area, pickup/drop-off patterns and time-slot demand | Where and when should operations focus? |

## KPI snapshot

The dashboard's headline cards display the following measures. Values are shown as presented in the report and should be interpreted in the context of the source dataset and its filters.

| KPI | Displayed value |
|---|---:|
| Total bookings | 93K |
| Lost bookings | 57K |
| Revenue | 52M |
| Total distance | 2.51M |
| Average distance | 24.64 |

Other report metrics include average revenue per booking, revenue per kilometre, booking completion/incompletion, customer cancellation, lost revenue, payment-method mix, and average customer/driver ratings.

## Tools and skills demonstrated

- **Power BI** — report layout, navigation, interactive visuals and filtering
- **DAX** — business measures and KPI calculations
- **Data modeling** — organizing ride-booking data for analysis
- **Business analytics** — translating operational data into questions and decisions
- **Data visualization** — time trends, comparative bars, KPI cards, tables and heatmap-style demand analysis

## Repository contents

The Power BI report (.pbix), presentation, insight report, and page screenshots were supplied for this project but are not yet included in this initial repository commit.

Suggested structure as the repository grows:

    uber-ride-analysis-powerbi/
    ├── README.md
    ├── docs/
    │   ├── dashboard-requirements.md
    │   └── insights-and-limitations.md
    ├── screenshots/
    │   ├── home.png
    │   ├── overview.png
    │   ├── vehicle.png
    │   ├── revenue.png
    │   ├── customer.png
    │   └── location.png
    └── report/
        └── Uber.pbix

## How to explore the report

1. Open the Power BI .pbix file in **Microsoft Power BI Desktop**.
2. Use the report's page navigation to move between Home, Overview, Vehicle, Revenue, Customer and Location.
3. Apply the available vehicle, time, and location filters where applicable.
4. Compare trends and breakdowns across pages rather than interpreting a single KPI in isolation.

The source dataset and refresh configuration are not included in this initial commit, so reproducing the exact figures may require the original data source and model configuration.

## Important interpretation notes

- KPI cards and charts may respond to report filters; values should be compared using consistent filter selections.
- “Lost bookings,” “lost revenue,” cancellation rates, and revenue risk depend on the definitions implemented in the report's measures.
- The supplied project documents describe the intended analysis. Exact calculation logic should be verified against the DAX measures and data model before using figures for operational decisions.
- This is an analytics portfolio project and should not be interpreted as an official Uber report.

## Acknowledgment

Documentation and review assistance was provided by **OpenAI ChatGPT**. The project owner is responsible for validating the report, measures, and business conclusions.

## Author

**Soumyadeep Podder**  
GitHub: [@Soumyadeepnsut](https://github.com/Soumyadeepnsut)

---

If you find an issue or have a suggestion, please open a GitHub issue with the page, metric, and steps to reproduce it.
