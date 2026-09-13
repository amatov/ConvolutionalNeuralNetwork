# Dependencies

## Matlab

No specific Matlab version is recorded. The `.m` scripts use:

- **Deep Learning Toolbox** -- `trainNetwork`, `layerGraph`,
  `trainingOptions`, `imageDatastore` (`Training_DeTraC.m`,
  `Training_original_classes.m`, `createLgraphUsingConnections.m`,
  `findLayersToReplace.m`). `Training_DeTraC.m` additionally requires
  the **Deep Learning Toolbox Model for ResNet-18 Network** add-on;
  `Training_original_classes.m` requires the **Deep Learning Toolbox
  Model for AlexNet Network** add-on.
- **Statistics and Machine Learning Toolbox** -- `pca` (`Pca_CXR.m`),
  `confusionmat`-style multi-class evaluation (`ConfusionMat_MultiClass.m`).
- **Image Processing Toolbox** -- `imadjust`, `stretchlim`, `imresize`
  (`readAndPreprocessImage.m`).

Both training scripts expect an `imageDatastore` folder (`dataset_A` /
`dataset_B`) of labeled training images that is not included in this
repository.

## Python

No `requirements.txt` is included. Scripts import: `torch` and
`deepchem` (`cnn.py`), `keras`/`tensorflow` (`CNN_test.py`,
`DeepLearning_Keras.py`, `mnist_convet.py`), `scikit-learn`
(`LogisticRegressionExample.py`), `xgboost` (`XGBoost_Model_test.py`),
`numpy`, `matplotlib`. `XGBoost_Model_test.py` expects a
`pima-indians-diabetes.csv` file, which is not included in this
repository.

`DeTraC_model.ipynb` uses a separate Python stack: OpenCV, pandas,
numpy, matplotlib, scikit-learn, scikit-image, mlxtend,
TensorFlow/Keras (`ResNet50`).

## R

Scripts require the **glmnet**, **imager**, and **readxl** packages
(`kerasMNISTconvnet.R`, `testMNISTconvnet.R`, `regressionUmiseq.R`,
`txttojpg.R`). `kerasMNISTconvnet.R`/`testMNISTconvnet.R` also use the R
`keras` package (a wrapper around the Python Keras/TensorFlow
installation).

## Hardcoded paths

Several `.m` files contain hardcoded absolute Windows paths to the
original author's machine, and `testMNISTconvnet.R`,
`regressionUmiseq.R`, and `txttojpg.R` reference hardcoded paths on a
specific HPC cluster (e.g. `~/genomedk/...`). Active (non-commented)
instances are flagged with an `% EDIT:` / `# EDIT:` comment directly
above them -- update these before running a script.
