Here's an updated version of your README with a more casual tone:

---

# SolarPowerPredictor

Hey there! This is a little side project I worked on as part of my learning journey. It's all about using a polynomial regression model to predict the solar intensity of solar panels based on local weather data. I found this super interesting and thought I'd give it a try!


## Weather Data Inputs

To make predictions, the model takes in the following weather data:

- Temperature
- Hours of daylight
- Humidity
- Precipitation
- Theoretical solar intensity, which depends on:
    - Latitude
    - Longitude
    - Day of year
    - Time of day (with 5-minute resolution)

## Output

The model gives two things as output:

1. **Predicted solar intensity** (in MW)
2. **Error score** compared to the actual solar panel data (so you can see how well the model's doing!)

## Assumptions

Here are a few things I assumed while working with the data:

- Temperature is in Celsius, but scaled by 1000. So, it’s parsed as a 3- or 4-digit number ending in "00".
- Visibility data is in "SM" and parsed as a number.
- Humidity is parsed as a 1- or 2-digit number, representing relative humidity in percentage.

## Sources

- **NOAA weather data files**: [NOAA FTP](ftp://ftp.ncdc.noaa.gov/pub/data/asos-fivemin/6401-2006)
- **Solar panel performance data**: [NREL Solar Power Data](https://www.nrel.gov/grid/solar-power-data.html)
