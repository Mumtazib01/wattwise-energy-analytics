# WattWise Energy Analytics Dashboard Layout

## 1. Project Overview
The dashboard is designed to provide an interactive view of household energy usage, identify peak demand periods, compare energy demand across regions, and support forecasting of future electricity consumption.

## 2. Dashboard Structure

### 2.1 Sidebar Controls
The left sidebar will contain all user controls for filtering data and customising the dashboard.

- Date range selector
- Metric selector
- Region focus selector
- Demand segment selector
- Season selector
- Forecast horizon slider

### 2.2 Main Header
The dashboard title and subtitle will be placed at the top of the page.

- Title: WattWise Energy Analytics Dashboard
- Subtitle: Interactive analysis of household energy demand, patterns, and forecasting

## 3. KPI Summary Cards
At the top of the dashboard, four KPI cards will display the most important metrics.

- Average load
- Peak demand
- Peak time
- Total observed load

These metrics allow users to quickly understand the current performance and identify high-demand periods.

## 4. Tabs Layout
The dashboard will use multiple tabs to keep the interface organised and easy to navigate.

### Tab 1: Overview
This tab provides an overall view of the selected metrics.

- Line chart of energy usage over time
- Histogram of selected metric distribution
- Box plot of energy demand by time band

### Tab 2: Patterns
This tab focuses on identifying demand patterns and relationships.

- Daily energy usage by region
- Heatmap of hourly demand by day of the week
- Scatter plot comparing selected metric with voltage

### Tab 3: Forecast
This tab displays future demand estimations.

- Forecast line chart with predicted demand
- Prediction interval or confidence band
- Brief summary of projected future energy demand

### Tab 4: Recommendations
This tab translates the analysis into actionable outputs.

- Average demand by segment
- Average load by region
- Energy efficiency story
- Recommended actions for reducing demand and improving efficiency

## 5. Visual Design Plan
The visual design should be clean, modern, and easy to interpret.

- Wide dashboard layout
- Light neutral background for readability
- Blue, orange, green, and teal chart colours for clarity
- Consistent titles, labels, and legends
- Use of Plotly interactive charts for filtering and hover inspection

## 6. User Experience Flow
1. User selects a date range and metric.
2. Sidebar filters update the dashboard results.
3. KPI cards refresh to show current performance.
4. Overview tab helps interpret overall consumption changes.
5. Patterns tab reveals peak periods and regional differences.
6. Forecast tab estimates future energy demand.
7. Recommendations tab suggests actions for reducing usage and planning ahead.

## 7. Expected Dashboard Outcome
The final dashboard should help users:

- understand electricity demand trends
- identify peak loading periods
- compare demand across regions and times of day
- forecast future energy consumption
- make informed decisions about efficiency and energy-saving strategies
