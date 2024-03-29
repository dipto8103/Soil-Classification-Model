## **Soil-Classification-Model**
**Features**

Image Preprocessing: Utilizes techniques such as image acquisition, low-pass filtering, Gabor filtering, and color quantization for preparing soil images for classification.
Feature Extraction: Extracts texture features from soil images using statistical parameters like mean amplitude, HSV histogram, and standard deviation.
Classification Model: Employs SVM for the classification of soils into various categories based on their textural and color features, aiming for high accuracy in distinguishing between types like Silty Sand, Sandy Clay, Peat, and others.
Dataset: The model is trained and evaluated on a dataset comprising 175 soil sample images, including categories such as Clay, Peat, Sandy Clay, and Silty Sand, among others. The dataset's diversity ensures the model's robustness and applicability to real-world soil analysis.

**Getting Started**

To use this model for soil classification:

Preparation:
Ensure all dependencies are installed and the dataset is accessible.

Execution: 
Run the Jupyter Notebook cells sequentially to perform image preprocessing, feature extraction, and classification.

Evaluation:
Analyze the classification results and accuracy metrics provided at the end of the notebook.

Dependencies:
Python 3.x,
Jupyter Notebook,
Scikit-learn,
NumPy,
OpenCV for Python,
Matplotlib (for visualization), TensorFlow libraries as needed.
