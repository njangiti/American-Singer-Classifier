# American Singer Classifier

This project is an image classification application that identifies five prominent American singers from photos using machine learning techniques.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Model Training](#model-training)
- [UI Development](#ui-development)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Overview

The American Singer Classifier project leverages computer vision and machine learning to classify images of five well-known American singers. The project involves data collection, preprocessing, feature extraction, model training, and deployment of an interactive user interface.

## Features

- **End-to-End Image Classification Pipeline:** Comprehensive pipeline from data collection to model deployment.
- **Advanced Feature Extraction:** Utilizes Haar Cascades for face and eye detection and wavelet transforms for feature enhancement.
- **User Interface:** Developed using PyCharm and HTML, allowing users to upload images and receive real-time predictions.
- **Model Evaluation:** Detailed evaluation using metrics such as accuracy, precision, and recall.
- **Deployment:** Application deployed for real-time use on Chrome.

## Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/njangiti/american-singer-classifier.git
    cd american-singer-classifier
    ```

2. **Create and activate a virtual environment:**
    ```bash
    python -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```

3. **Install the required packages:**
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. **Run the application:**
    ```bash
    jupyter notebook americansingerclassifier.ipynb
    ```

2. **Open the notebook in your browser and follow the steps to upload an image and get the singer's classification.**

## Technologies Used

- **Programming Language:** Python
- **Libraries:** OpenCV, scikit-learn, PyWavelets
- **Development Environment:** PyCharm, Jupyter Notebook
- **Web Technologies:** HTML

## Project Structure

american-singer-classifier/
│
├── data/
│ ├── raw/ # Raw image data
│ ├── processed/ # Processed image data
│
├── notebooks/
│ ├── americansingerclassifier.ipynb # Main Jupyter Notebook
│
├── models/
│ ├── saved_model.pkl # Trained model
│ ├── class_dictionary.json # Class labels
│
├── ui/
│ ├── index.html # HTML for user interface
│
├── requirements.txt # Required Python packages
├── README.md # Project README file
└── LICENSE # Project License


## Model Training

The model training process involves several steps:

1. **Data Collection and Preprocessing:** Images are collected and preprocessed to ensure consistency.
2. **Feature Extraction:** Haar Cascades are used for face and eye detection, and wavelet transforms are applied for feature enhancement.
3. **Model Selection and Training:** Multiple models (SVM, Random Forest, Logistic Regression) are trained and evaluated.
4. **Model Evaluation:** The best performing model is selected based on evaluation metrics.

## UI Development

The user interface is developed using HTML and PyCharm, providing an interactive platform for users to upload images and receive predictions.

1. **HTML Interface:** Simple and intuitive interface for image upload.
2. **Integration with Model:** Backend integration to process the uploaded image and return the prediction.

## Results

The model's performance is evaluated using a confusion matrix and other metrics. The final model achieves high accuracy in classifying the images of the five singers.

![Confusion Matrix](path_to_confusion_matrix_image)

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. **Fork the repository.**
2. **Create a new branch:**
    ```bash
    git checkout -b feature-branch
    ```
3. **Commit your changes:**
    ```bash
    git commit -m 'Add some feature'
    ```
4. **Push to the branch:**
    ```bash
    git push origin feature-branch
    ```
5. **Submit a pull request.**

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
