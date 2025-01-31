# yolov5-fruit-vegetable-detection
YOLOv5-powered object detection model for recognizing fruits and vegetables.
# Fruit and Vegetable Classification with YOLOv5

This project aims to classify fruits and vegetables using the YOLOv5 object detection model. The model was trained on a dataset obtained from **Roboflow**, and **TensorBoard** was used to visualize the training results. The project was implemented in a **Google Colab** environment using **Python**.

## Table of Contents
1. [Project Description](#project-description)
2. [Data](#data)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Training Results Visualization](#training-results-visualization)
6. [License](#license)
7. [Contributing](#contributing)
8. [Acknowledgements](#acknowledgements)

## Project Description
This project uses the **YOLOv5** (You Only Look Once version 5) object detection model to classify fruits and vegetables. YOLOv5 is an advanced and efficient deep learning model that detects objects in real-time. The dataset used for training the model is from **Roboflow**, which provides various labeled datasets for machine learning tasks.

The project is implemented using **Python** in a **Google Colab** environment to ensure flexibility and computational power. The training process and results are visualized using **TensorBoard**, which helps track the model's performance over time.

## Data
The dataset for this project is sourced from **Roboflow**. It includes images of various fruits and vegetables, labeled with the respective class names. The dataset is suitable for training an object detection model to recognize and classify different food items.

You can access the dataset on **Roboflow**: [Roboflow Dataset](https://roboflow.com).

## Installation

Follow these steps to set up and run the project:

1. Clone the repository:
   ```bash
   git clone https://github.com/BeyzaDurdu/fruit-vegetable-detection.git
   cd fruit-vegetable-detection
2. Install the required Python libraries:

pip install -r requirements.txt
(Optional) Set up Google Colab: Open the project in Google Colab and follow the instructions in the notebook.

Usage
1- Run the YOLOv5 training script to train the model:
python train.py --img 640 --batch 16 --epochs 50 --data fruit_vegetables.yaml --weights yolov5s.pt

2- After training, use the model to make predictions on new images:
python detect.py --weights runs/train/exp/weights/best.pt --img 640 --source path_to_your_images

3- Visualize the training process using TensorBoard:
tensorboard --logdir=runs
License
This project is licensed under the MIT License - see the LICENSE file for details.
Contributing
Contributions are welcome! If you would like to contribute, please fork the repository and submit a pull request.

Acknowledgements
Thanks to Roboflow for providing the dataset: Fruit and Vegetable Dataset.
The model is implemented using YOLOv5 and trained on Google Colab for easy execution and powerful computational resources.
TensorBoard was used for tracking and visualizing the training process.
