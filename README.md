## ConvolutionalNeuralNetwork

Classification and detection of multiple myeloma with deep learning.

## Quick start

This repository contains Matlab, Python, and R scripts for machine
learning and deep learning classification experiments. See
[DEPENDENCIES.md](DEPENDENCIES.md) for the required Matlab toolboxes,
Python packages, and R packages.

## Repository contents

- `Training_DeTraC.m`, `Training_original_classes.m`,
  `createLgraphUsingConnections.m`, `findLayersToReplace.m`,
  `construct_dataset_B.m`, `extract_features.m`, `Pca_CXR.m`,
  `ConfusionMat_MultiClass.m`, `readAndPreprocessImage.m` -- Matlab
  deep-learning classifier training and feature analysis.
- `DeTraC_model.ipynb` -- a Python/TensorFlow-Keras ResNet50
  classification notebook.
- `cnn.py`, `CNN_test.py`, `DeepLearning_Keras.py`,
  `LogisticRegressionExample.py`, `XGBoost_Model_test.py` -- standalone
  Python model examples (PyTorch/deepchem, Keras/TensorFlow,
  scikit-learn, XGBoost).
- `kerasMNISTconvnet.R`, `testMNISTconvnet.R`, `mnist_convet.R`,
  `regressionUmiseq.R`, `txttojpg.R` -- R scripts for Keras-in-R
  examples and genomics data preparation and regression analysis.
- [`figures/`](figures/) -- a figure of the CNN network architecture I prepared.
- **License:** see [LICENSE](LICENSE) -- research/educational use.

## About

I tested several deep learning and machine learning classification approaches (Keras/TensorFlow, PyTorch/DeepChem, scikit-learn, XGBoost) for multiple myeloma drug-efficacy classification, including the DeTraC COVID-19 chest X-ray classification algorithm (ResNet18) developed by the lab of Mohamed Gaber; for detailed information, see: https://www.researchgate.net/publication/382850918_Analysis_of_Multiple_Myeloma_Drug_Efficacy

Method from the lab of Mohamed Gaber - Asmaa Abbas, Mohammed M. Abdelsamea, Mohamed Medhat Gaber "Classification of COVID-19 in Chest X-ray Images Using DeTraC Deep Convolutional Neural Network" (2021), https://pubmed.ncbi.nlm.nih.gov/34764548/; code: https://github.com/asmaa4may/DeTraC_COVId19/tree/master/python_code
