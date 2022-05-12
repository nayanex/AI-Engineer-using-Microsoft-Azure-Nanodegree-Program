# Building Computer Vision Solutions with Azure

## New Terms

Today, Azure Cognitive Services are delivered under four umbrella service categories:

* Decision
* Language
* Speech
* Vision

* **Azure Cloud:** A collection of various services, tools, and technologies for you to develop and deploy enterprise applications all in the cloud in a quick, secure, and low-cost way.
* **Azure Cognitive Services:** A collection of various AI tools and technologies to build intelligent and supported algorithms into applications and websites to provide the ability to see, hear, speak, understand, and interpret information to meet your business requirements.
* **Azure Custom Vision (CV) services:** A collection of AI services to process image analysis solutions for your custom business and personal requirements.

## Business Stakeholders

An end-to-end machine learning (ML) pipeline consists of three stages:

* Data preparation
* Model training
* Model consumption and monitoring

Here are the key stakeholders in this pipeline:

* **You, the AI engineer:** Mostly focus on completing machine learning training and generating the final business-ready model. You will be involved in all 3 stages of the ML pipeline and work with the following 3 teams listed below.
* **Data engineering team:** Responsible for data generation and collection and making sure the data is ready for machine learning. This team mostly focuses on data preparation.
* **DevOps team, or MLOps:** Combining DevOps with machine learning process management, this team ensures your machine learning training process is optimal and meets the speed required for completing the tasks. This team mostly focuses on model training.
* **Business team: **Look at the model performance through various metrics and confirm if the model is ready for the business to consume. This team will eventually use the results from the model. This team mostly focuses on model consumption and monitoring.

## Jupyter Notebook Workspace Instructions

If you have multiple images, you can either upload them one-by-one into the folder, or upload a zipped folder and unzip it using the following code in the Jupyter Notebook:

```python
import zipfile
with zipfile.ZipFile('ENTER PATH TO ZIP FILE HERE', 'r') as zip_ref:
 zip_ref.extractall('ENTER DIRECTORY TO EXTRACT TO')
```

Here is an example:

```python 
import zipfile
with zipfile.ZipFile('/home/workspace/nature-images.zip', 'r') as zip_ref:
 zip_ref.extractall('/home/workspace/nature-images')
```

## Using Jupyter Notebooks in Your Local Environment

If you want to download the Jupyter Notebook and work on it locally instead, you need to install the **Azure Core Python SDK** as well as the Azure service-specific SDK to use the relevant Azure services.

Here are the commands for installing the Azure Core and service-specific Python SDKs:

Azure Core Python SDK: `pip install azure-core`
Azure Cognitive Services: `pip install azure-mgmt-cognitiveservices`
Azure Form Recognizer: `pip install azure-ai-formrecognizer`
Azure Face service: `pip install azure-cognitiveservices-vision-face`
Azure Computer Vision: `pip install azure-cognitiveservices-vision-computervision`
Azure Custom Vision: `pip install azure-cognitiveservices-vision-customvision`
Azure Video Analyzer: `pip install azure-mgmt-videoanalyzer`
Video Indexer third-party SDK: `pip install video-indexer`

**Note:** You may need to install other third-party packages depending on each individual Jupiter Notebook you will be using.

## Local Environment Setup

You could also download the Local Environment Setup File from the `Local Environment Setup File` folder and use the `environment.yml` file to install all the Python packages at once to set up your local environment. Refer to these [instructions](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file) for creating an environment from an environment.yml file.

```
# Create the environment from the environment.yml file:
conda env create -f environment.yml
# Activate the new environment 
conda activate ai-azure-c1
# Verify that the new environment was installed correctly
conda env list
```

Once the environment is set up and you've installed the [Anaconda](https://www.anaconda.com/products/distribution), you can download the Jupyter notebooks from this [Github repo](https://github.com/udacity/cd0461-building-computer-vision-solutions-with-azure-exercises).