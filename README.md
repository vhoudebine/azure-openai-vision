# GPT4 Turbo with Vision for Image classification

This repository walks through the usage of GPT4 Turbo with Vision on Azure Open AI to classify documents.

The repository contains two notebooks:
- [Data preprocessing](./data_preprocessing.ipynb): reads the PDF documents as images, crops them to the zone of interest and writes the cropped images to the [extracted_stamps](./extracted_stamps/) folder.

- [GPT4 Vision Evaluation](./gpt4_vision_eval.ipynb): reads the cropped images, classifies them using GPT4 on Azure OpenAI and evaluates the prediction against the ground truth labels (obtained from parsing the image paths).

## Quickstart

### 1. Install dependencies

System dependencies for OpenCV
```sudo apt-get install ffmpeg libsm6 libxext6  -y```

Python libraries required for both notebooks

```pip install -r requirements.txt```

### 2. Provide your Azure credentials
Create a `.env` file based on the [.env.example](./.env.example) file, replace the placeholders with your account information.

### 3. Execute the Data preprocessing notebook
### 4. Execture the GPT4 Vision Eval notebook