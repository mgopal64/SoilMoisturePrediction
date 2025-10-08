# SoilMoisturePrediction
# MHACKS 2025:

Farmers need timely, local soil moisture insights to optimize irrigation, reduce watering cost, and boost yields.

NASA's SMAP satellite provides global soil moisture data, but at coarse resolution (36 km, every 2–3 days)—not detailed or frequent enough for field-level farm decisions.

I fuse NASA SMAP satellite data with high-resolution land models (STF_SSM) and local weather data (from Visual Crossing) to create 1 km, 3-hourly soil moisture predictions.
Using Random Forest, I combine:

STF_SSM soil moisture maps (1 km, 3-hourly)
Local weather features (temperature, rainfall, humidity, solar radiation, etc.)
Feature engineering to capture rainfall events, drying trends, and more

This project researches into if local weather features could be predictors for soil moisture as sensed by SMAP in conjunction with STF_SSM.

Yielded that soil moisture is highly autocorrelated but IS correlated with local humidity. Random Forest R^2 = 0.84, MSE = 0.02.



