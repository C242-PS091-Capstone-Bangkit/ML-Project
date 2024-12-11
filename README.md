# Machine Learning Project - Google Colab Implementation 🚀

This project demonstrates a machine learning workflow using Google Colab and datasets stored in Google Drive.

## Requirements
The project uses the following libraries:
- `os`
- `pickle`
- `random`
- `numpy`
- `tensorflow`
- `matplotlib`
- `ipywidgets`
- `PIL` (Pillow)
- `sklearn`
- `torchvision`

Ensure that these libraries are installed before running the project.

## Setup Instructions

### 1. Prepare the Dataset
1. **Upload the Dataset to Google Drive**:  
   - Place your dataset folder in the `My Drive` section of your Google Drive.  
   - For example, if your dataset folder is named `dataset`, its path should look like this:  
     ```
     /content/drive/My Drive/dataset
     ```

2. **Mount Google Drive in Colab**:  
   Add the following code to your notebook to mount Google Drive:  
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   dataset_path = '/content/drive/My Drive/dataset'
