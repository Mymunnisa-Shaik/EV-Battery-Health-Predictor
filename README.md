# EV Battery Health Predictor

## Project Overview

This project analyzes the capacity degradation of an electric vehicle battery using NASA battery aging data. It calculates State of Health (SOH) and explores machine learning models to estimate battery health based on discharge cycle number.

## Objectives

* Analyze battery capacity degradation across discharge cycles.
* Calculate battery State of Health (SOH).
* Visualize battery health degradation.
* Compare machine learning models for SOH prediction.

## Dataset

* **Source:** NASA Prognostics Center of Excellence (PCoE)
* **Battery:** B0005
* **Data used:** Battery discharge cycles and measured capacity.

## Tools and Technologies

* Python
* Google Colab
* NumPy and Pandas
* Matplotlib
* SciPy
* Scikit-learn

## Work Completed

* Loaded and processed NASA battery aging data.
* Extracted discharge-cycle capacity values.
* Calculated SOH relative to the initial measured capacity.
* Plotted capacity degradation and SOH trends.
* Trained and compared Linear Regression, Polynomial Regression, and Random Forest models.
* Created a simple cycle-based SOH prediction.

## Experimental Results

For the chronological train-test evaluation, Linear Regression achieved an MAE of approximately **1.66 SOH percentage points** and an R² score of approximately **-2.055**.

These results indicate that the model has limitations when predicting future battery health. The current model uses discharge cycle number as its only input.

## Limitations

* The prediction uses only discharge cycle number.
* Model performance on future cycles needs improvement.
* The prediction is experimental and is not suitable for real-world battery diagnosis.

## Future Improvements

* Include voltage, current, temperature, and other battery parameters.
* Improve model validation and future-cycle prediction.
* Explore additional machine learning models.
* Develop a simple user interface for battery health estimation.

## Disclaimer

This is an educational portfolio project using public research data. The predictions are experimental and should not be used as a substitute for real-world battery diagnostics.
