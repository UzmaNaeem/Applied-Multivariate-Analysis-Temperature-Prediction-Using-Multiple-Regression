
# Applied Multivariate Analysis: Temperature Prediction Using Multiple Regression

## Summary
The "Applied Multivariate Analysis Temperature Prediction Using Multiple Regression" project aims to predict temperature variations based on multiple predictor variables, including time of day, pressure, relative humidity, dew point, and their interaction terms. The dataset consists of 60 observations collected from an open-source historical weather API.

## Explanation of Data
The dataset includes the following variables:
- **Time of Day**: An indicative variable representing different times of the day.
- **Pressure**: Atmospheric pressure measured in hPa.
- **Relative Humidity**: The percentage of humidity at a height of 2 meters.
- **Dew Point**: The temperature at which air becomes saturated and condensation occurs, measured at 2 meters above ground level.
- **Apparent Temperature**: A measure of how hot it feels, considering humidity and wind.
- **Windspeed**: The speed of the wind in meters per second.
- **Cloud Cover**: The fraction of the sky covered by clouds.

## Results/Key Findings
The multiple regression analysis was conducted in a backward stepwise manner, starting with all six predictor variables. Here are the key findings from the regression analysis:

### Significant Variables:
- Time of Day
- Pressure
- Relative Humidity
- Dew Point

### Insignificant Variables:
- Apparent Temperature
- Windspeed
- Cloud Cover

### Regression Models:
1. **1st Regression (All Variables)**:
   - R² = 0.886, Adjusted R² = 0.871, Standard Error = 1.121

2. **2nd Regression (Excluding Apparent Temperature)**:
   - R² = 0.886, Adjusted R² = 0.873, Standard Error = 1.111

3. **3rd Regression (Excluding Apparent Temperature & Windspeed)**:
   - R² = 0.881, Adjusted R² = 0.870, Standard Error = 1.126

4. **4th Regression (Excluding Apparent Temperature, Windspeed & Cloud Cover)**:
   - R² = 0.877, Adjusted R² = 0.868, Standard Error = 1.133

5. **5th Regression (Including Interaction Terms)**:
   - R² = 0.890, Adjusted R² = 0.876, Standard Error = 1.099

### Durbin-Watson Statistic:
The Durbin-Watson statistic of 1.631 indicates no significant autocorrelation among the residuals.

## Conclusion
The project successfully used multiple regression analysis to predict temperature based on significant meteorological variables, including time of day, pressure, relative humidity, and dew point. The final model, incorporating interaction terms, achieved an R² of 0.890, indicating a strong fit. The Durbin-Watson statistic confirmed no significant autocorrelation among the residuals. This demonstrates the effectiveness of multiple regression for temperature prediction and suggests potential for further refinement with additional variables or modeling techniques.
