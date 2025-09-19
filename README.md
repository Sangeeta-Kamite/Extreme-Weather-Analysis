# Extreme-Weather-Analysis
This project analyzes daily weather station data to detect and visualize extreme weather events. It combines threshold-based detection, streak analysis, and interactive visualizations to provide a deeper understanding of temperature patterns, extreme events, and long-term trends.

Project Goals
- Detect and classify extreme weather days based on defined thresholds
- Analyze heatwave and cold snap streaks (persistence of extremes)
- Explore temporal patterns: daily, monthly, yearly trends
- Compare stations to evaluate geographic variation in weather extremes

Dataset Sources
- Daily Weather Data: Contains daily max/min temperature, wind speed, and precipitation
- Station Metadata: Includes station ID, name, and location details
- Thresholds File: Defines extreme conditions (e.g., tmax_f > 95°F, tmin_f < 32°F)

Features Analyzed
- Temperature: Daily max/min, moving averages, extreme hot/cold days
- Precipitation: Extreme rainfall events
- Wind Speed: High wind event detection
- Extreme Flags: Binary indicators for hot, cold, windy, or rainy extremes
- Streaks: Multi-day sequences of extreme events (heatwaves, cold snaps)

Technologies Used
- Python – Core analysis
- Pandas & NumPy – Data cleaning & transformation
- Matplotlib & Plotly – Static & interactive visualizations
- Statsmodels – Trend and regression analysis
- Jupyter Notebook – Exploratory data analysis workflow

Methods Implemented
1. Data Cleaning & Preprocessing
   - Handle missing values, parse dates, convert data types

2. EDA (Exploratory Data Analysis)
   - Summary statistics, missing value heatmaps, yearly coverage

3. Extreme Event Detection
   - Apply thresholds to classify days as extreme

4. Streak Analysis
   - Identify heatwave and cold snap streaks (≥3 days)
   - Visualize streak length distributions with histograms

5. Rolling Window Analysis
   - Rolling 7-day sum of extreme days

6. Monthly & Yearly Trends
   - Aggregate metrics by month and year
   - Linear regression for trend detection

7. Station Comparisons
   - Interactive dropdowns to compare stations across months

Key Insights & Findings
- Extreme events cluster in multi-day streaks (heatwaves and cold snaps)
- Monthly analysis highlights seasonal variation in extremes
- Stations show geographic differences in temperature and extreme day counts
- Rolling 7-day windows provide better visibility into short-term climate risks

Performance Metrics
- Counts of extreme days per year and month
- Length of longest heatwave/cold snap streaks
- % of total days flagged as extreme
- Slope of monthly/annual trendlines with statistical significance

Impact & Applications
- Climate Research – Evaluate frequency & severity of extreme weather events
- Urban Planning – Support climate adaptation strategies
- Energy & Utilities – Anticipate demand surges during heatwaves/cold snaps
- Insurance & Risk Management – Assess climate-related risks for assets and operations

Example Visualizations
- Interactive daily temperature with moving average
- Bar charts of extreme days by year/month
- Line charts of rolling 7-day extreme days
- Histograms of heatwave/cold snap streak lengths
- Station-level comparisons with interactive dropdowns

Future Work
- Add geospatial visualizations (map of stations with extreme day counts)
- Build a Streamlit dashboard for live interaction
- Incorporate real-time weather APIs for continuous monitoring

