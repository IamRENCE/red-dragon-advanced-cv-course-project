<!-- Tempalate README.md extracted from https://github.com/othneildrew/Best-README-Template/tree/master -->

<a name="readme-top"></a>

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <h3 align="center">Red Dragon AI Advanced Computer Vision Course Project Submission</h3>

  <p align="center">
    Ship Vessels Recognition
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

The model is fine-tuned using a pre-trained YOLOv11 model (`yolo11n.pt`) to enhance detection accuracy while minimizing training time. This pre-trained model was selected due to its transfer learning capabilities, allowing it to leverage pre-existing knowledge from large datasets, such as COCO, for improved generalization to our specific use case.

### The Project Workflow:

- **Model Training & Evaluation**: The YOLOv11 model is fine-tuned on the custom dataset, with evaluation metrics based on the trained model's performance on the validation set.
- **Inference**: The final model is tested on nine random images from the test set, and the results demonstrate that the fine-tuned model performs well, with accurate detection of both civilian and warship objects.
- **Video Tracking**: In the final step, video tracking is applied to detect and track civilian and warship objects across video frames. Using maritime surveillance videos from YouTube (MP4s Files: [1](https://www.youtube.com/watch?v=BTIrd4OBdzo&ab_channel=HarvestTechnology), [2](https://www.youtube.com/watch?v=iNgl7MoHxk0&ab_channel=SilentSentinel), [3](https://www.youtube.com/watch?v=yTxM6Exl9p4&ab_channel=CovertCabal)), both BoT-SORT and ByteTrack trackers are evaluated for their effectiveness in maintaining object identity and tracking moving targets over time.

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
