<!-- Tempalate README.md extracted from https://github.com/othneildrew/Best-README-Template/tree/master -->

<a name="readme-top"></a>

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <h3 align="center">Red Dragon AI Advanced Computer Vision Course Project Submission</h3>

  <p align="center">
    Singlish to English Translation
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about-the-project">About The Project</a></li>
    <li><a href="#prerequisites">Prerequisites</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->

## About The Project

This project focuses on detecting civilian and warship objects in images using a YOLO-based model. The primary objective is to develop a robust object detection model that can be used for surveillance and defense purposes.

The dataset for training, validation, and testing is sourced from [Mcships GitHub repository](https://github.com/ZhengYitong2333/Mcships). This dataset has been converted into the YOLO format using the provided script in the data source's respository.

The model is fine-tuned using a pre-trained YOLOv5 model (`yolo11n.pt`) to improve detection accuracy and reduce training time. This pre-trained model was selected for its effectiveness in transfer learning, leveraging pre-existing knowledge from large datasets like COCO for better generalization to our specific use case.

### The Project Workflow:

- **Model Training & Evaluation**: The YOLOv5 model is fine-tuned on the custom dataset, with evaluation metrics based on the trained model's performance on the validation set.
- **Inference**: The final model is tested on nine random images from the test set, and the results demonstrate that the fine-tuned model performs well, with accurate detection of both civilian and warship objects.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Prerequisites

Install the required packages under `requirements.txt`.

Make sure to have CUDA (^12.6) and cuDNN installed for the notebook to run on GPU.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->

## Acknowledgments

Thanks to Martin and Sam for the guidance throughout this course!

- [Red Dragon AI Pte Ltd](https://reddragonai.com/)
  - [Martin Andrews](mailto:martin@reddragon.ai)
  - [Sam Witteveen](mailto:martin@reddragon.ai)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
