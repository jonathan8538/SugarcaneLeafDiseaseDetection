# SugarcaneLeafDiseaseDetection
This project aims to classify sugarcane leaf disease using svm ( with GridSearchCV and baseline)
The workflow is divided into several parts:
1) Dataset augmentation (rotating, flip and constrast jitter) -> to provide more information for the model to learn
2) Image preprocessing -> convert to grayscale, resize and contrast enhancement
3) Feature extraction -> GLCM features (contrast, correlation, energy, homogeneity), color features ( rgb mean and standard deviation), ViT features
4) Filtering best features ( 300 features from all extracted features)
5) Model training ( 1 version with GridSearchCV and 1 more with SVM baseline)
