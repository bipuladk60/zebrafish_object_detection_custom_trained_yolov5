# Zebrafish Egg Stage Detection with YOLOv5

## Project Overview
This project aims to develop an object detection model using YOLOv5 to identify and classify the developmental stages of zebrafish eggs. Zebrafish (*Danio rerio*) are widely used in biological research, and understanding their developmental stages can provide valuable insights for studies in genetics, developmental biology, and toxicology.

## Current Progress
In the current phase of this project, the YOLOv5 model has been trained to detect and classify zebrafish eggs into seven categories:
- **Advanced**
- **Dead**
- **Empty**
- **Holder**
- **Returned**
- **Stage 1 (Zygote)**
- **Stage 2-4 (Cleavage)**

Although the model can accurately classify Stage 1 (Zygote) and Stage 2-4 (Cleavage) eggs, it does not yet cover the later developmental stages, including:
- Blastula
- Gastrula
- Segmentation
- Pharyngula
- Hatching
- Larval
- Juvenile
- Adult

The current dataset does not include labeled data for these stages, which limits the model's ability to classify eggs beyond the Zygote and Cleavage stages.

## Future Goals
With access to a more comprehensive dataset that includes all developmental stages of zebrafish eggs, this model could be expanded to accurately detect and classify all stages. Such a dataset would allow the model to provide more detailed insights into the development process, which could be useful in a variety of research and educational settings.

## Dataset
The dataset used for this project includes labeled images for seven classes, as listed above. However, it does not yet contain annotations for all developmental stages of zebrafish. Future iterations of the project will require a more extensive dataset with labels for each stage to improve classification accuracy and expand the model's capabilities.

## Model
This project uses YOLOv5, a state-of-the-art object detection model known for its speed and accuracy. YOLOv5 is well-suited for real-time applications and can perform object detection efficiently on complex images.

### Model Performance
The trained YOLOv5 model demonstrates high accuracy in detecting the current seven classes. Below are some performance metrics:
- **Precision**: 0.878
- **Recall**: 0.952
- **mAP@0.5**: 0.963
- **mAP@0.5:0.95**: 0.843

These metrics indicate that the model performs well in its current form and could be further improved with additional data.

## Results
The following images demonstrate the model's predictions versus the ground truth labels:

<p align="center">
  <img src="https://github.com/user-attachments/assets/5935961a-c4ff-4ceb-aea9-c4f7c6d72c4b" alt="Predicted" width="400"/>
  <img src="https://github.com/user-attachments/assets/ab20f935-0c73-4e70-b555-951608fddd50" alt="Ground Truth" width="400"/>
</p>

<p align="center">
  <strong>Left:</strong> Predicted | <strong>Right:</strong> Ground Truth
</p>


##Acknowledgement
roboflow:
  workspace: phdproject-b58ng
  project: zebrafish-database
  version: 20
  license: CC BY 4.0
  url: https://universe.roboflow.com/phdproject-b58ng/zebrafish-database/dataset/20
