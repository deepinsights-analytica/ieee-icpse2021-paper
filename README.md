# Prediction of Energy Consumption for Variable Customer Portfolios Including Aleatoric Uncertainty Estimation
### Oliver Mey<sup>1</sup>, André Schneider<sup>1</sup>, Olaf Enge-Rosenblatt<sup>1</sup>, Yesnier Bravo<sup>2</sup>, Pit Stenzel<sup>2</sup>
##### <sup>1</sup>Fraunhofer IIS/EAS, Fraunhofer Institute for Integrated Circuits, Division Engineering of Adaptive Systems, Dresden, Germany<br><sup>2</sup>Bettergy S.L., R&D Department, Málaga, Spain

This GitHub repository is part of a paper submission to the **10th International Conference on Power Science and Engineering (ICPSE 2021)** held on Oct. 21-23, 2021 in Yildiz Technical University, Istanbul, Turkey (preprint: http://arxiv.org/abs/2110.02166). It contains a series of five freely available Python Jupyter notebooks with code examples. The code was used to get the prediction results described within the ICPSE paper. The dataset used for training and validation of the neural network along with this study is available via the Fraunhofer Fordatis database (https://fordatis.fraunhofer.de/handle/fordatis/215). This dataset contains energy consumption values of 499 anonymized customers located in Spain for the year 2019 in hourly resolution. In addition, temperature values corresponding to the zip code-exact location of each customer was part of the dataset. Both, the Python code and the data, allow all interested engineers, data scientists, and Machine Learning / Deep Learning / AI freaks to check the prediction results described in the IEEE paper and to supplement their own analyzes. We look forward to your comments and suggestions for improvements.

![Results for an example customer from the validation dataset in daily resolution (upper part) and in hourly resolution for randomly selected example
days.](figures/figure_5.png)
*Results for an example customer from the validation dataset in daily resolution (upper part) and in hourly resolution for randomly selected example
days.*

#### Notebooks

**![A1_DataExploration.ipynb](notebooks/A1_DataExploration.ipynb)**
The notebook reads the available datasets (energy consumptions, weather data, customer profiles) and illustrates the time series using a few examples.

**![A2_DataExploration.ipynb](notebooks/A2_DataExploration.ipynb)**
The notebook implements a *DataLoader* class for a more efficient reading of the data and metadata. 

**![A3_DataExploration.ipynb](notebooks/A3_DataExploration.ipynb)**
The notebook reads the available data using the *DataLoader* class and prepares the data for further feature extraction.

**![B1_Feature Extraction.ipynb](notebooks/B1_FeatureExtraction.ipynb)**
The notebook demonstrates the feature extraction using a view examples. It implements a powerful *FeatureExtractor* class.

**![C1_ModelTraining.ipynb](notebooks/C1_ModelTraining.ipynb)**
The notebook reads the data, extracts the needed feature vectors and trains a complex prediction model. Selected results for predicting the energy consumption for the next day are shown.

