# Machine Learning Project - Google Colab Implementation 🚀

This project demonstrates a machine learning workflow using Google Colab and datasets stored in Google Drive.
The Skin Type and Skin Condition model is built both from scratch and using transfer learning with the **InceptionV3** pretrained model. **The fixed model used in this capstone project is the InceptionV3 model due to its superior accuracy compared to other models.**

## Requirements
The project uses the following libraries:
- `os`
- `pickle`
- `random`
- `numpy`
- `tensorflow`
- `matplotlib`
- `ipywidgets`
- `sklearn`
- `torchvision`

Ensure that these libraries are installed before running the project.

## Setup Instructions

### 1. Prepare the Dataset
1. **Upload the Dataset to Google Drive**:  
   - Place the dataset folder in the `My Drive` section of your Google Drive.  
   - For example, if dataset folder is named `dataset`, its path should look like this:  
     ```
     /content/drive/My Drive/dataset
     ```

2. **Mount Google Drive in Colab**:  
   Add the following code to your notebook to mount Google Drive:  
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   dataset_path = '/content/drive/My Drive/dataset'

### 2. Open the Project in Google Colab
1. Visit Google Colab and open a new notebook.
2. Upload the `.ipynb` file for this project to Colab environment.

### 3. Install Required Libraries

### 4. Pre-Process The Dataset
1. **Load images from the dataset folder**: Use the path specified earlier to load images.
2. **Split the dataset into training and validation dataset**
3. **Dataset Augmentation**: To improve model performance and reduce overfitting, augment the dataset with transformations such as rotation, flipping, scaling, or color adjustments.

### 5. Build and Train The Model
    - Define the machine learning model using TensorFlow
    - Train the model using the prepared dataset.

### 6. Evaluate the Model
Evaluate the performance of the trained model using metrics such as accuracy, confusion matrix, or classification report. Follow the evaluation steps provided in the notebook.

### 7. Additional Notes
Use GPU runtime in Colab for faster computation:
- Go to Runtime > Change runtime type.
- Select GPU as the hardware accelerator.

