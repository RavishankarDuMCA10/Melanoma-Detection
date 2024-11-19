# Melanoma Detection
> To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
### Algorithm Used

Convolutional Neural Network

### Dataset Information
The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

The data set contains the following diseases:

- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

<img width="625" alt="Screenshot 2024-11-18 at 11 14 24 PM" src="https://github.com/user-attachments/assets/dc8a2b47-47cf-46a7-958e-18f4b38a4afe">

### Sample Images from Dataset

<img width="736" alt="Screenshot 2024-11-18 at 11 12 05 PM" src="https://github.com/user-attachments/assets/921483ce-ba38-450f-a5ee-45238b7f423d">


## Steps involved
- Importing all the important libraries
- Data Loading and Create datasets
- Visualize one instance of all the nine classes present in the dataset
- Baseline Model Building
- Training the Model and Visualizing training results
- Building an augmented model
- Training the augmented model and Visualizing training results
- Checking and rectifing Class Imbalance with augmentor
- Building the final model
- Training the final model and Visualizing training results
- Verifying the model

## Results

### Baseline Model

#### Baseline Model Architecture

<img width="603" alt="Screenshot 2024-11-18 at 11 12 19 PM" src="https://github.com/user-attachments/assets/ca119f98-787f-4e7f-b21f-66493e1e7a7f">


Accuracy and loss charts for Baseline Model:

<img width="710" alt="Screenshot 2024-11-18 at 11 12 33 PM" src="https://github.com/user-attachments/assets/5a24f466-28ad-47d7-a743-436dc4acb543">

### Augmented Model

#### Augmented Model Architecture

<img width="293" alt="Screenshot 2024-11-19 at 12 19 41 PM" src="https://github.com/user-attachments/assets/12809b10-2a0e-4fc6-8f25-21ac14d4a271">


Accuracy and loss charts for Augmented Model:

<img width="737" alt="Screenshot 2024-11-18 at 11 14 12 PM" src="https://github.com/user-attachments/assets/e177d9e0-5bbb-41b6-8694-332e6658bb6b">

### Final Model

#### Final Model Architecture

<img width="318" alt="Screenshot 2024-11-19 at 12 20 58 PM" src="https://github.com/user-attachments/assets/d370be67-2ca4-44c8-85a2-75846b63d12f">


Accuracy and loss charts for Augmented Model:

<img width="724" alt="Screenshot 2024-11-18 at 11 14 45 PM" src="https://github.com/user-attachments/assets/3c4f0b26-9937-474c-a89f-5ea15ad88609">


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- **Improved Performance:** Training accuracy improved significantly, reaching 93.61% by the end of training. Validation accuracy also improved to 85.33%, with validation loss steadily decreasing.

- **Addressing Underfitting:** Early epochs (1–10) showed underfitting, as both training and validation accuracies were low. However, as training progressed, the model learned meaningful patterns, reducing underfitting.

- **Overfitting Trends:** Overfitting appears minimal since the validation accuracy remains close to the training accuracy, and the validation loss follows a consistent downward trend.

- **Class Rebalancing Impact:** After class rebalancing (weighted loss, data augmentation, or oversampling) applied, it helped to reduce biases in predictions, resulting in better generalization across classes, as evidenced by consistent validation accuracy improvement.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- tensorflow - version 2.16.2
- matplotlib - version 3.9.2
- numpy - version 1.26.4
- pandas - version 2.2.3
- keras - version 3.6.0
- PIL - version 11.0.0
- Augmentor - version 0.2.12
<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by the need for efficient melanoma detection.
- References:
  https://www.isic-archive.com/
  https://challenge2020.isic-archive.com/
- This project was based on [Convolutional Neural Networks](https://learn.upgrad.com/course/5800/segment/55852/333576/1009197/5042300).

## Contact
Created by [@RavishankarDuMCA10] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
