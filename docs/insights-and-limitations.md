# KPI Interpretation and Validation Notes

This document separates visible dashboard figures from conclusions that still require checking the Power BI model.

## Headline figures shown in the supplied dashboard

| Metric | Displayed value |
|---|---:|
| Bookings | 93K |
| Lost bookings | 57K |
| Revenue | 52M |
| Total distance | 2.51M |
| Average distance | 24.64 |

These are rounded values read from the dashboard screenshots. They are not independently recalculated from the source dataset and may vary with filters.

## Questions the dashboard is designed to investigate

- Which vehicle categories contribute most to revenue and bookings?
- How do bookings and revenue vary by month or quarter?
- Which payment methods account for the most revenue?
- Which customer segments and cancellation patterns may indicate retention risk?
- Which pickup/drop areas and time slots show high activity?
- How much revenue is associated with incomplete or cancelled rides?

These are analytical questions, not verified findings by themselves. Validate conclusions against the underlying model and data before presenting them as facts.

## Validation checklist

### Metric definitions
- Document the exact numerator and denominator for completion, incompletion, and cancellation rates.
- Confirm how “Lost Bookings” is defined and whether it is mutually exclusive from other booking statuses.
- Confirm how “Lost Revenue” and “Customer Revenue Risk” are estimated.
- Verify whether average distance is per booking, completed ride, or another population.
- Confirm revenue currency and distance units.

### Data and model
- Confirm the dataset's source, date coverage, row count, and refresh steps.
- Check missing values, duplicate booking identifiers, invalid distances, and negative or null revenue.
- Verify relationships among booking, customer, vehicle, location, payment, and date fields.
- Check whether date slicers use a continuous date table.

### Visuals and interaction
- Test monthly and quarterly toggles.
- Test vehicle, time, and location filters across all pages.
- Check sorting of month names and ranking of category charts.
- Validate bookmark-based show/hide filter controls.
- Confirm that totals in tables agree with headline cards under the same filters.

## Limitations

The supplied screenshots and requirements document describe the report's visible design and intended functionality. The source data, DAX definitions, and model relationships have not been independently audited in this documentation. Therefore, this repository does not claim that the dashboard's business conclusions have been externally validated or that it represents an official Uber report.
