# Machine Learning Project - Model Implementation 🚀

This project demonstrates a machine learning workflow using Google Colab and datasets stored in Google Drive. The Skin Type and Skin Condition model is built both from scratch and using transfer learning with the InceptionV3 pretrained model. The fixed model used in this capstone project is the InceptionV3 model due to its superior accuracy compared to other models. Additionally, we perform fine-tuning on the InceptionV3 model to improve its performance by training it on our specific dataset, allowing the model to adjust its weights for better accuracy on skin type and skin condition classification tasks.

## Requirements📋
The project uses the following libraries:
- `os`
- `pickle`
- `random`
- `numpy`
- `tensorflow`
- `matplotlib`
- `sklearn`
- `torchvision`
- `from google.colab import files`

Ensure that these libraries are installed before running the project.

## Setup Instructions⚙️

### 1. Open the Project in Google Colab🌐
- At the top of the notebook file on GitHub, you should see a badge saying "Open in Colab" provided. This allows anyone with access to the repository to open the notebook in Google Colab with a simple click and then make a copy to your drive, or
- Visit Google Colab and open a new notebook.
- Upload the `.ipynb` file for this project to Colab environment.


### 2. Prepare the Dataset
1. **Upload the Dataset to Google Drive**📥:  
   - Place the dataset folder in the `My Drive` section of your Google Drive.  
   - For example, if dataset folder is named `dataset`, its path should look like this:  
     ```
     /content/drive/My Drive/dataset
     ```

2. **Mount Google Drive in Colab**🔗:  
   Add the following code to your notebook to mount Google Drive:  
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   dataset_path = '/content/drive/My Drive/dataset'

   
### 3. Install Required Libraries🧰


### 4. Pre-Process The Dataset📸
- **Load images from the dataset folder**: Use the path specified earlier to load images.
- **Split the dataset into training and validation dataset**
- **Dataset Augmentation**: To improve model performance and reduce overfitting, augment the dataset with transformations such as rotation, flipping, scaling, or color adjustments.


### 5. Build and Train The Model 🏋️‍♂️
- Define the machine learning model using TensorFlow
- Train the model using the prepared dataset.


### 6. Evaluate the Model📊
Evaluate the performance of the trained model using metrics such as accuracy, confusion matrix, or classification report. Follow the evaluation steps provided in the notebook.


### 7. Additional Notes📝
Use GPU runtime in Colab for faster computation:
- Go to Runtime > Change runtime type.
- Select GPU as the hardware accelerator.

