# MSI-MSS-tumor-prediction
The project is using combination of transfer learning models (Inception V3, Resnet 50, Inception-Resnet V2) and machine learning classifiers (SVM, MLP, Random Forest) to predict the tumor status of the colon cancer based on histopathological samples.

Dataset used for this project:
Kather, J. N., 2019. Histological images for MSI vs. MSS classification in gastrointestinal cancer, FFPE samples. [Online] Available at: https://zenodo.org/record/2530835#.Y1fEBHbMKUn

The original dataset comprises a total of 192,312 histological images. This project used reduced dataset consisting of 88,335 samples (60,000 samples for training, 28,335 for test).

Environment used to run the code:
	Software:
		-Kaggle Notebook
		-Python 3.7
		-Tensorflow 2.3.0
		-Sklearn 1.2.0
	Hardware:
		-GPU: NVIDIA T4x2 16GB
		-CPU: Intel Xeon 2.2GHz x4 32GB
		-RAM: 30GB

Directories:
	Classification:
		Contains Jupyter Notebook with Python code used to train classification models.
  Demo:
		Contains demonstration of the final classification model.
  Feature Extraction:
		Contains Jupyter Notebook with Python code used to extract the features from fine-tuned models.
  Transfer Learning:
		Contains Jupyter Notebooks with Python code used to perform training and fine-tuning of pre-trained models

Reproducing the results:
	1.Transfer Learning (~40h using NVIDIA T4 x2 to train and fine-tune all models)
  2.Feature extraction (~20h using NVIDIA T4 x2 to extract the features from training and test datasets)
  3.Classification (~30h using NVIDIA T4 x2 & Intel Xeon to train all classification models)
