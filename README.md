# Predictive Japan Earthquake Model

## Team Members
- Priyanka Patil (pp673)
- Alex Hoang (ah3756)
- Vijval Vemula (vv354)
- Mohamed Shehaf Aakil Sharfudeen (ms5475)

## Project Overview
This project aims to develop a predictive model for estimating the magnitude of earthquakes in Japan using various spatial and temporal features. The model helps in understanding the underlying patterns and contributing factors of seismic activity in the region.

## Data Description
The input data consists of features describing the characteristics, location, and context of earthquake events in Japan, including:
- `time`: Timestamp of the earthquake occurrence.
- `latitude`: North-south position of the earthquake epicenter.
- `longitude`: East-west position of the earthquake epicenter.
- `depth`: Depth of the earthquake epicenter.
- `mag`: Magnitude of the earthquake.
- `magtype`: Type of magnitude scale used.
- `nst`: Number of seismic stations reporting.
- `gap`: Largest azimuthal gap between seismograph stations.
- `dmin`: Closest station distance to the earthquake.
- `rms`: Root mean square of the amplitude spectrum.
- `net`: Seismic network reporting the earthquake.
- `id`: Identifier for the earthquake event.
- `updated`: Timestamp when the earthquake data was last updated.
- `place`: Location description of the earthquake.
- `type`: Type of seismic event.
- `horizontalerror`: Horizontal error of the earthquake location.
- `deptherror`: Error in the depth measurement.
- `magerror`: Error in the magnitude measurement.
- `magnst`: Number of seismic stations used to calculate magnitude.
- `status`: Status of the earthquake event.
- `locationsource`: Source of the earthquake location data.
- `magsource`: Source of the earthquake magnitude data.
- `significant_earthquake`: Flag indicating if the earthquake is significant.
- `magtype_mb`, `magtype_ms`, `magtype_mw`, `magtype_mwb`, `magtype_mwc`, `magtype_mwr`, `magtype_mww`: Different types of magnitude measures.
- `distance_to_tokyo`, `distance_to_osaka`, `distance_to_kyoto`: Distances from earthquake epicenter to specific cities.
- `seismic_energy`: Amount of energy released during the earthquake.

## Predictive Modeling
The goal is to predict the magnitude of the next earthquake using the following models:
- **Gradient Boosting Regressor (GBR)**
- **Neural Networks (using TensorFlow)**
- **Support Vector Machines (SVM)**

### Gradient Boosting Regressor (GBR)
Gradient boosting is used to build a strong predictive model by combining multiple weak learners (decision trees) sequentially. Hyperparameters such as the number of estimators, learning rate, and maximum depth are tuned using grid search cross-validation.

### Neural Networks
A neural network model with multiple dense layers is implemented using TensorFlow. The network captures complex patterns in the data through its layered structure and non-linear activation functions.

### Support Vector Machines (SVM)
SVMs perform classification by finding the hyperplane that best separates different classes in feature space. Kernels like linear and RBF are used to capture non-linear relationships.

## Evaluation Metrics
The models are evaluated using the root mean squared error (RMSE) metric on the test set. The ground truth represents the observed values of the target variable (earthquake magnitudes).

## Installation
To install the required dependencies, use the `requirements.txt` file:
```bash
pip install -r requirements.txt
````

## Usage
1. Preprocess the data and extract relevant features.
2. Train the predictive models using the training dataset.
3. Evaluate the models using the test dataset and compare performance based on RMSE and other metrics.

## Conclusion
The project demonstrates the application of various predictive modeling techniques to estimate earthquake magnitudes. The results provide insights into the factors contributing to seismic activity and the effectiveness of different models.

## Contributions
| Section | Writing | Editing |
|---------|---------|---------|
| Predictive Modeling Problem Definition | Alex | Alex, Vijval |
| Predictive Models | Aakhil | Priyanka, Vijval |
| Evaluations | Priyanka | Aakhil, Alex |
| Appendix | Vijval | Priyanka, Aakhil |

# earthquake-prediction-using-machine-learning
