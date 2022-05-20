# Identify Azure Cognitive Services

Here’s an overview of the computer vision-related Azure Cognitive Services:

* **Azure Computer Vision:** Optical Character Recognition (OCR), layout & text extraction, image understanding, spatial analysis
* **Azure Custom Vision:** Image classification and object detection
* **Azure Face Services:** Face detection, face recognition, emotion, and sentiment
* **Azure Video Analyzer/Indexer:** Brand detection, text extraction/speech transcription, language identification, people in video (face identification and recognition), emotion and sentiment extraction
* **Azure Form Recognizer:** Layout recognizer, text recognizer, specific content (ID, receipts) recognition
* **Azure's Data Storage Resources**
    * Azure Blob Storage for objects or files
    * Azure SQL Server for structured information
    * Azure Cosmos DB for unstructured information or key-value pairs

## Identify Azure Cognitive Services

Here is a list of different Azure Cognitive Services and technologies that will be used in our UdaciMart example:

* **Customer identification:**
    * Azure Face Services for face detection and face recognition
* **Item label identification:**
    * Azure Form Recognizer
* **Item identification:**
    * Azure Video Analyzer/Indexer for brand recognition
* **Identification verification:**
    * Azure Form Recognizer to extract information from ID Cards
* **Customer emotion and sentiment:**
    * Azure Video Analyzer/Indexer
* **Storefront capacity:**
    * Spatial Analysis for headcount
* **Social distancing management:**
    * Spatial Analysis
    * Azure Custom Vision (Spatial Analysis can use Custom Vision models if needed)
* **Customer assistance and feedback:**
    * Video _Analyzer/Indexer_ for text, sentiment, and emotion extraction from video

## Cognitive Resources and a Storage Account

To begin with, you should set up the following resources:

1. [Face Recognition Service](https://azure.microsoft.com/en-in/services/cognitive-services/face/)
2. [Form Recognizer Service](https://azure.microsoft.com/en-in/services/form-recognizer/#overview)
3. [Computer Vision Cognitive Service](https://azure.microsoft.com/en-in/services/cognitive-services/computer-vision/)
4. [Azure Video Analyzer/Indexer](https://azure.microsoft.com/en-us/products/video-analyzer/#overview)
5. [Storage Account](https://docs.microsoft.com/en-us/azure/storage/common/storage-account-overview)

You can find detailed instructions on creating [Cognitive Services resource](https://docs.microsoft.com/en-us/azure/cognitive-services/cognitive-services-apis-create-account?tabs=multiservice%2Cwindows?WT.mc_id=udacity_learn-wwl?) in the Microsoft docs.

By the end of the current course, your Azure resources page would show the following resources:

![Azure Resources for the exercises. You can have different resource names.](https://video.udacity-data.com/topher/2022/April/625410f9_screenshot-2022-04-11-at-4.58.27-pm/screenshot-2022-04-11-at-4.58.27-pm.jpeg)

### Face Cognitive Service

Navigate to the **Cognitive Services** in the Azure portal.

![Choose the Face API in the Cognitive Services](https://video.udacity-data.com/topher/2022/April/6253f779_screenshot-2022-04-11-at-2.11.54-pm/screenshot-2022-04-11-at-2.11.54-pm.jpeg)

Search and create a Face API using the following basic configuration:

**Section**	| **Field**	| **Value**
------------|-----------|-----------
**Basics**	| Resource Group | Use existing
 |Region 	| Use a consistent value, say East US 2
 | |Name	| Your choice
 | |Pricing tier	| Free

Leave the remaining section/fields as default and click on the "Review & Create" button. On successful validation, create the Face API resource.

![Creating Face Cognitive Service](https://video.udacity-data.com/topher/2022/April/6253f6ce_screenshot-2022-04-11-at-3.06.59-pm/screenshot-2022-04-11-at-3.06.59-pm.jpeg)

Use a similar configuration to create other Cognitive Service resources.

* Computer vision for analyzing content in images and videos.
* Custom vision for a customized image recognition model. We have described this one on the upcoming page.

![Try creating the Computer vision and Custom vision resources](https://video.udacity-data.com/topher/2022/April/62540969_screenshot-2022-04-11-at-3.33.24-pm/screenshot-2022-04-11-at-3.33.24-pm.jpeg)

## VSCode Regular Expression

https://docs.microsoft.com/en-us/visualstudio/ide/using-regular-expressions-in-visual-studio?view=vs-2022

