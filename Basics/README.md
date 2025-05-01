# COVID-19 Analytics Dashboard

## Overview

This project is a Streamlit-based dashboard that visualizes COVID-19 data stored in Snowflake. It provides interactive analytics including key metrics, geographic distribution, and temporal trends of COVID-19 cases worldwide.

## Features

- **Real-time Data Visualization**: Connects directly to Snowflake data warehouse
- **Interactive Analytics**:
  - Top 10 affected countries by confirmed cases
  - Time-series analysis of cases and deaths
  - 7-day moving average calculation
- **Key Metrics Dashboard**:
  - Total confirmed cases
  - Total deaths
  - Average death rate
- **Date Range Filtering**: Explore data for specific time periods

## Technical Stack

- **Frontend**: Streamlit (Python)
- **Data Warehouse**: Snowflake
- **Data Processing**: Snowpark Python API
- **Visualization**: Streamlit native charts

## Setup Instructions

1. **Prerequisites**:
   - Python 3.7+
   - Snowflake account with proper permissions
   - Streamlit installed (`pip install streamlit`)

2. **Install dependencies**:

   ```bash
   pip install snowflake-snowpark-python pandas
   ```

3. **Configuration**:
   - Set up your Snowflake connection in Streamlit's secrets.toml file
   - Ensure the `COVID_CLEANED` table exists in your Snowflake database

## Usage

1. **Data Quality Report**: Verify the raw data in the expandable section
2. **Key Metrics**: View summary statistics at the top
3. **Trends Analysis**:
   - Geographic tab shows country distribution
   - Temporal tab shows cases over time with moving average
4. **Filters**: Adjust date range in the sidebar

## Troubleshooting

- If visualizations fail, check:
  - Column names match between SQL queries and DataFrame operations
  - Data exists in the specified date ranges
  - Snowflake connection is properly configured

## Future Enhancements

- Add more detailed regional breakdowns
- Incorporate vaccination data
- Implement predictive modeling
- Add export functionality for reports

## License

This project is open-source and available under the MIT License.
