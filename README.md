# Learning about Time Series Anomaly Detection

Related Resources
- [Video: A review of machine learning techniques for anomaly detection - The Alan Turing Institute](https://youtu.be/LRqX5uO5StA)

## 1) Data
We want to use an open source dataset with sensor data to start learning about different preprocessing and modeling techniquesbut these are hard to come by for infrastructure! Luckily, there is a [Kaggle dataset for pump sensor data](https://www.kaggle.com/nphantawee/pump-sensor-data) which we can use to get started.

### Data Cleaning and Normalization
Before we get started we'll want to remove or interpolate to fill NaN values. Also consider scaling data to the same scale.

## 2) Exploratory Data Analysis
The first thing we should do is some EDA to understand the data and investigate correlations between the different inputs and the outputs we're interested in.

## 3) Preprocessing Options
These are some preprocessing techniques we may want to consider before actually modeling

### Dimentionality Reduction
Depending on the number of input features, we may want to condense them into a more concise signal to reduce the dimensionality of our problem space. Some techniques may include:

- **Principle Component Analysis (PCA)**
    - [A Visual Explaination of PCA](https://setosa.io/ev/principal-component-analysis/)
    - [A One-Stop Shop for Principal Component Analysis](https://towardsdatascience.com/a-one-stop-shop-for-principal-component-analysis-5582fb7e0a9c)


## 4) Modeling

### Potential Approaches

- **LSTM AutoEncoder (Self-Supervised)**
    Long Short Term Memory AutoEncoders are a type of self-supervised recurrent neural network (RNN)
    - [LSTM for Predictive Maintenance on Pump Sensor Data](https://towardsdatascience.com/lstm-for-predictive-maintenance-on-pump-sensor-data-b43486eb3210)
    - [Paper and Code: LSTM-based Encoder-Decoder for Multi-sensor Anomaly Detection](https://paperswithcode.com/paper/lstm-based-encoder-decoder-for-multi-sensor): There seems to be a good implimentation with PyTorch linked here

### Training & Testing
It's important to avoid over-fitting your model to the test data by not going back and tuning your parameters on the training set to get a better output on the test set. 

## 5) Deploying the Model

## 6) Alerting