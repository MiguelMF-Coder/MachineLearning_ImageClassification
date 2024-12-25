# **Animal Breed Classification Project**

## **Project Overview**
This project implements an animal breed classification system using machine learning models. The primary focus is on developing a pipeline that can handle both segmented and non-segmented images to improve classification accuracy in real-world scenarios. The key components of the project include:

- Preprocessing and data augmentation.
- Implementation of a classification model for non-segmented images.
- A planned hybrid pipeline for segmentation and classification to handle noisy backgrounds.

Currently, the non-segmented image classification model has been fully implemented and trained. Due to time constraints, the segmentation-based models remain untrained but are intended for future development.

---

## **Features**

- **Non-Segmented Image Classification**: A trained model capable of accurately predicting animal breeds from raw images.
- **Segmentation-Based Classification Pipeline (Planned)**: Future implementation to combine segmentation and classification for enhanced accuracy.
- **Real-World Applicability**: Designed to handle noisy and diverse backgrounds.

---

## **Setup and Installation**

### **Step 1: Clone the Repository**
```bash
git clone <repository_url>
cd <repository_name>
```

### **Step 2: Set Up Environment**
1. Install Conda if not already installed. You can download it from [Miniconda](https://docs.conda.io/en/latest/miniconda.html).

2. Create a Conda environment:
   ```bash
   conda create -n breed_classifier python=3.10
   conda activate breed_classifier
   ```

3. Install dependencies from `requirements.txt`:
   ```bash
   pip install -r requirements.txt
   ```

### **Step 3: Download Pretrained Model**
The pretrained model for non-segmented image classification can be downloaded from the following link:
[Download Model](<model_download_link>)

Save the model file (`Best_Non-Segmented_Classifier.pth`) in the project directory.

### **Step 4: Prepare the Dataset**
Ensure the dataset is organized as follows:
```
data/
  └── oxford-iiit-pet/
      └── images/
          ├── image1.jpg
          ├── image2.jpg
          └── ...
```
You can download the Oxford-IIIT Pet dataset from [here](https://www.robots.ox.ac.uk/~vgg/data/pets/).

---

## **Usage**

### **Run the Prediction Script**
To process and classify images, place the images in the `Img_Prueba` folder and run the script:
```bash
python script.py
```

The script will:
1. Predict the breed of each image.
2. Optionally display a reference image from the dataset for comparison.
3. Print a summary of predictions and their distribution.

### **Results**
The results, including predicted classes, will be displayed on the console. You can modify the script to save these results in a file if needed.

---

## **Future Work**

- **Train Segmentation-Based Models**: Develop and train models for segmenting noisy images.
- **Pipeline Integration**: Combine segmentation and classification for dynamic decision-making based on image complexity.
- **Performance Evaluation**: Test the system in real-world scenarios with high variability.

---

## **Acknowledgements**

- Oxford-IIIT Pet Dataset.
- PyTorch and torchvision libraries.
- OpenAI for providing tools and support.

---

## **Contributing**
Feel free to fork this repository, raise issues, or submit pull requests to improve the project.

---

## **License**
This project is licensed under the MIT License. See the `LICENSE` file for details.
