This project aims to classify sugarcane leaf diseases using Support Vector Machine (SVM), both with baseline parameters and with hyperparameter tuning via GridSearchCV.

Workflow Overview:
1) Dataset Augmentation
Techniques applied: rotation, flipping, and contrast jittering, to increase data diversity and help the model learn better

2) Image Preprocessing
Steps include converting to grayscale, resizing, and contrast enhancement

3) Feature Extraction

Texture features: GLCM (contrast, correlation, energy, homogeneity)

Color features: RGB mean and standard deviation

Deep features: ViT features

4) Feature Selection
The top 300 most relevant features from all extracted features

5) Model Training

Baseline SVM: Trained with default parameters

SVM with GridSearchCV: Trained with optimized hyperparameters

6) Model Evaluation

Baseline SVM achieved 94% accuracy

GridSearchCV-tuned SVM achieved 97% accuracy
Note: The difference may be influenced by random sampling done in data splitting.

