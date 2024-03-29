## **Soil-Classification-Model**
**Features**

Image Preprocessing: Utilizes techniques such as image acquisition, low-pass filtering, Gabor filtering, and color quantization for preparing soil images for classification.
Feature Extraction: Extracts texture features from soil images using statistical parameters like mean amplitude, HSV histogram, and standard deviation.
Classification Model: Employs SVM for the classification of soils into various categories based on their textural and color features, aiming for high accuracy in distinguishing between types like Silty Sand, Sandy Clay, Peat, and others.
Dataset: The model is trained and evaluated on a dataset comprising 175 soil sample images, including categories such as Clay, Peat, Sandy Clay, and Silty Sand, among others. The dataset's diversity ensures the model's robustness and applicability to real-world soil analysis.


## Running the Soil Classification Model from Colab to Local Environment

This guide provides detailed instructions for running the soil classification model locally, which was initially developed in Google Colab. The model employs Support Vector Machine (SVM) for classifying soil types based on image data.

### Preparing Your Local Environment

#### Step 1: Install Python and Jupyter Notebook
Ensure you have Python 3.x and Jupyter Notebook installed on your local machine. If not, you can download Python from [the official site](https://www.python.org/downloads/) and install Jupyter Notebook using pip:
```bash
pip install notebook
```

#### Step 2: Clone the GitHub Repository
Clone or download the GitHub repository containing the `.ipynb` file and any accompanying files (like the `requirements.txt` for Python dependencies).

#### Step 3: Install Required Libraries
Navigate to the repository's root directory in your terminal or command prompt and install the required Python libraries. If a `requirements.txt` file is provided, use the following command:
```bash
pip install -r requirements.txt
```
If not, install the necessary libraries individually:
```bash
pip install scikit-learn numpy opencv-python matplotlib
```

### Running the Notebook Locally

#### Step 1: Start Jupyter Notebook
In your terminal or command prompt, navigate to the cloned repository's directory and start Jupyter Notebook:
```bash
jupyter notebook
```

#### Step 2: Open the `.ipynb` File
In the Jupyter interface that opens in your browser, navigate to and open the `.ipynb` file (e.g., `ReNewed_Soil_Classification_Model.ipynb`).

#### Step 3: Execute the Notebook
Run the notebook cells in sequence by pressing `Shift + Enter` for each cell or using the "Run" button in the toolbar. Follow any additional instructions or comments within the notebook.

### Handling Images for Classification

#### Downloading and Preparing Images
- **Image Source:** Ensure you have access to the images you wish to classify. If the project includes a dataset or images, follow the provided links or instructions to download them.
- **Image Format:** Check the notebook or project documentation for any specific requirements regarding image format, size, or preprocessing steps.

#### Reading Images in the Notebook
- Modify any file paths in the notebook to point to the location of your images on your local machine. This typically involves changing variables or parameters in the code cells responsible for loading images.
- If the notebook includes Colab-specific commands for file upload (e.g., `from google.colab import files`), you'll need to replace or remove these commands. Instead, use OpenCV (`cv2.imread()`) or similar libraries to read images from your filesystem.

### Additional Notes
- **Compatibility:** Ensure your local Python environment matches the one used in Colab (e.g., Python version and library versions) for compatibility.
- **Data and Model Paths:** Adjust any paths used in the notebook for loading datasets, images, or models to match your local directory structure.

By following these steps, you should be able to run the soil classification model on your local machine, using your images for classification. Remember, the key to a smooth transition from Colab to a local environment is ensuring that all dependencies are correctly installed and that file paths are appropriately set.
