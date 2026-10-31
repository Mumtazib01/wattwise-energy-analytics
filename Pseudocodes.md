# WattWise Energy Analytics: Pseudocode

## 1. Algorithm Pseudocode

```text
ALGORITHM EnergyConsumptionAnalysis
    INPUT: household_energy_dataset
    OUTPUT: insights, visualisations, forecast, recommendations

    LOAD dataset
    INSPECT dataset structure and column names
    CHECK for missing values, invalid entries, and date format issues

    IF data quality issues are found THEN
        CLEAN data
        CONVERT date-time fields to correct format
        HANDLE missing values
        REMOVE duplicated or inconsistent rows
    END IF

    CREATE new time-based features:
        hour
        day_name
        month
        season
        time_band

    ANALYSE consumption trends over time
    CALCULATE summary statistics:
        mean load
        peak load
        peak time
        total observed load

    IDENTIFY periods of high energy demand
    COMPARE usage by region and time band

    IF forecasting is feasible THEN
        BUILD time-series forecast model
        PREDICT future energy usage for selected number of days
    END IF

    GENERATE charts and dashboard views
    CREATE recommendations for energy-saving actions

    DISPLAY final results
END ALGORITHM
```

## 2. Program Pseudocode

```text
PROGRAM WattWiseApp
    INITIALISE application environment
    SET page configuration for dashboard
    DEFINE file paths and constants

    LOAD cleaned dataset from storage

    IF dataset cannot be loaded THEN
        DISPLAY error message
        STOP program
    END IF

    PREPARE dataset for analysis:
        SORT by datetime
        ADD derived features
        CREATE seasonal labels

    DISPLAY sidebar controls:
        date range
        energy metric
        region focus
        time band
        season
        forecast horizon

    GET user-selected inputs
    FILTER dataset based on selected criteria

    IF no valid records remain THEN
        DISPLAY warning message
        STOP processing current view
    END IF

    CALCULATE KPIs
    GENERATE overview charts
    GENERATE pattern analysis charts
    GENERATE forecasting chart
    DISPLAY recommendations

    RUN dashboard continuously until user exits
END PROGRAM
```

## 3. Process Pseudocode

```text
PROCESS DataAnalysisWorkflow
    STEP 1: Import raw energy dataset
    STEP 2: Validate dataset fields and structure
    STEP 3: Clean data and standardise formats
    STEP 4: Derive time features
    STEP 5: Filter data based on business questions
    STEP 6: Compute descriptive statistics
    STEP 7: Visualise trends and comparisons
    STEP 8: Test forecasting model if needed
    STEP 9: Interpret results and create insights
    STEP 10: Prepare final recommendations
    STEP 11: Publish results in dashboard or report
END PROCESS
```

## 4. Machine Learning Pseudocode

```text
ML_PSEUDOCODE ForecastEnergyDemand
    INPUT: cleaned_energy_data, forecast_days
    OUTPUT: predicted_demand, confidence_interval

    GROUP data by day
    CALCULATE daily average energy consumption

    IF total daily records < 2 THEN
        RETURN "Forecast cannot be generated"
    END IF

    SELECT features:
        date
        daily_energy_usage

    SPLIT data into training and validation sets
    INITIALISE forecasting model

    SET model parameters:
        yearly_seasonality = TRUE
        weekly_seasonality = TRUE
        daily_seasonality = FALSE

    TRAIN model on historical data
    GENERATE future dates for forecast_days
    PREDICT future energy demand
    COMPUTE lower and upper prediction bounds

    EVALUATE performance using validation metrics
    DISPLAY forecast chart and summary results
END ML_PSEUDOCODE
```

## 5. Dashboard (Streamlit and Tableau) / Application Pseudocode

### 5.1 Streamlit Application Pseudocode

```text
STREAMLIT_APP WattWiseDashboard
    LOAD dataset
    CHECK dataset validity

    SET page layout to wide format
    SET title to "WattWise Energy Analytics"

    CREATE sidebar with controls:
        date range selector
        metric selector
        region selector
        demand segment selector
        season filter
        forecast horizon slider

    READ user selections
    FILTER dataset according to selected criteria

    IF filtered data is empty THEN
        DISPLAY warning message
        STOP rendering charts
    END IF

    CALCULATE peak demand, average load, and total usage
    SHOW KPIs in summary cards

    DISPLAY tab 1: Overview
        line chart of energy usage over time
        histogram of selected metric
        box plot across time bands

    DISPLAY tab 2: Patterns
        daily energy usage by region
        daily/hour heatmap

    DISPLAY tab 3: Forecast
        forecast line chart
        prediction interval

    DISPLAY tab 4: Recommendations
        practical actions based on demand patterns

    UPDATE dashboard automatically when user changes filters
END STREAMLIT_APP
```

### 5.2 Tableau Application Pseudocode

```text
TABLEAU_APP EnergyInsightsDashboard
    CONNECT to cleaned_energy_dataset
    CREATE data source
    DEFINE date field as datetime
    DEFINE metrics as:
        global_active_power
        global_reactive_power
        voltage
        global_intensity
        sub_metering_1
        sub_metering_2
        sub_metering_3

    CREATE calculated fields:
        hour
        day_of_week
        season
        time_band

    BUILD worksheets:
        line chart for consumption over time
        bar chart for peak periods
        heatmap for hourly demand by day
        scatter plot for relationship analysis

    ADD dashboard filters:
        date range
        region
        time segment
        season

    DESIGN dashboard layout with KPI cards and charts
    ADD narrative insights and recommendations panels
    PUBLISH dashboard for stakeholder review
END TABLEAU_APP
```

## Final Summary

These pseudocode sections show the full lifecycle of the WattWise Energy Analytics project:

- algorithm design for the analysis process
- main program structure
- business process flow
- machine learning forecasting logic
- interactive dashboard application logic in Streamlit and Tableau

Together, we represent the end-to-end workflow from raw data to actionable energy insights.
