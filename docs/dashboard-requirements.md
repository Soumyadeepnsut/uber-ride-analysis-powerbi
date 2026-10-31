# Dashboard Requirements and Page Guide

This guide is based on the supplied *Uber Power BI Dashboard — Business Requirements & Page-wise Functional Explanation* document and the dashboard screenshots.

## 1. Home page

**Purpose:** Introduce the project and provide a clear entry point.

**Elements**
- Uber branding and a short description of the ride-hailing analytics use case.
- Navigation to Home, Overview, Vehicle, Revenue, Customer, and Location.

**Business value:** Establishes context before users explore the report and makes page navigation straightforward.

## 2. Overview page

**Purpose:** Give executives and managers a high-level operational snapshot.

**Headline KPIs**
- Total Bookings
- Lost Bookings
- Total Revenue
- Total Distance
- Average Distance

**Analysis**
- Monthly and quarterly booking and revenue trends.
- Revenue by vehicle type.
- Top pickup and drop locations.
- Average customer and driver ratings.

**Controls:** Vehicle-type filter and month/quarter toggles.

## 3. Vehicle page

**Purpose:** Compare vehicle-level performance.

**Metrics**
- Booking count
- Revenue generated
- Revenue contribution percentage
- Completion rate
- Incomplete rate

The page includes a vehicle-level detail table and monthly completed-booking sparklines. It is intended to help identify high-contributing vehicle categories and inform fleet, pricing, and incentive decisions.

## 4. Revenue page

**Purpose:** Understand revenue generation and potential revenue at risk.

**Analysis dimensions**
- Monthly and quarterly revenue trends, including month-over-month change.
- Revenue by vehicle type.
- Top revenue-generating customers.
- Revenue by payment method: UPI, cash, wallet, credit card, and debit card.
- Lost revenue, revenue per kilometre, and average revenue per booking.

## 5. Customer page

**Purpose:** Explore customer segments, cancellations, and potential retention issues.

**Segments**
- First-time customers
- Return customers
- Regular customers

**Metrics and analysis**
- Customer cancellation rate
- Customer revenue risk percentage
- Customer cancelled count
- Estimated revenue impact of customer cancellations
- Top cancellation reason
- Customer trends by month/quarter
- Payment-method preference
- Customer-level detail table

## 6. Location page

**Purpose:** Understand geographical and temporal demand patterns.

**Analysis**
- Total distance by vehicle type and area.
- Active pickup areas.
- Busy time slots and day/hour demand heatmap.
- Monthly and quarterly distance trends.

These views can inform driver allocation, peak-period planning, and location-level operational decisions.

## Global usability requirements

The supplied requirements describe:
- Consistent navigation and icons across pages.
- Page-level and report-level filtering.
- Vehicle, time, and location filters where relevant.
- A hide/show filter panel controlled through Power BI bookmarks.

## Validation checklist

Before using the dashboard for business decisions, verify:
- DAX definitions for completed, lost, and incomplete bookings.
- Whether cancellation counts overlap with lost-booking counts.
- The denominator used for every rate and percentage.
- Revenue currency and distance units.
- Date-table relationships and month/quarter sorting.
- Filter interactions and bookmark behavior.
- Whether the displayed KPI values change as expected under filters.
