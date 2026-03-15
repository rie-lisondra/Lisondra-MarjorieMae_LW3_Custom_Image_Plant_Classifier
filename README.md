# Lisondra-MarjorieMae_LW3_Custom_Image_Plant_Classifier

---

## Activity 3: Guide Questions (Student Reflection & Explanation) 

## 1. Dataset Preparation 
- ### How did you organize your dataset in Google Drive?
  <div align="justify">
    The dataset was stored in the ImageDataset folder on Google Drive. Within this folder, images were organized into separate subfolders corresponding to each aquatic plant species, including <i>arrow_arum, blue_flag_iris, bulrush_scirpus</i>, and others. All images of a given species were placed in its respective folder. TensorFlow automatically interprets these folders as labels when loading the dataset using <b>image_dataset_from_directory()</b>.
  </div>

- ### Why is folder structure important for TensorFlow image loading?
  <div align="justify">
    The folder structure is important because TensorFlow uses the folder names as class labels when loading images. When the function <b>image_dataset_from_directory()</b> is used, TensorFlow scans the dataset directory and treats each subfolder as a separate category. If the folder structure is incorrect or images are mixed into a single folder, TensorFlow will not be able to assign the correct labels to the images, which will affect model training and accuracy.
  </div>

   <div align="justify">
  </div>
  
## 2. Model Training 
- ### What is the role of convolutional layers in image classification?
  <div align="justify">
    Convolutional layers extract critical visual features from images by detecting patterns such as edges, shapes, textures, and colors. Early layers capture simple features like lines and curves, whereas deeper layers identify more complex patterns, including object shapes. These extracted features enable the model to differentiate between image classes during classification.
  </div>
  
- ### Why do we split data into training and validation sets?
  <div align="justify"> 
    The dataset is divided into training and validation sets to assess the model's performance on unseen data. The training set enables the model to learn to recognize patterns in images. The validation set is employed during training to evaluate the model's ability to classify new images not included in the training process. This approach helps identify issues such as overfitting, where the model memorizes training data instead of learning generalizable patterns. 
  </div>

## 3. Performance Analysis 
- ### What accuracy did your model achieve?
   <div align="justify">
     The model achieved approximately <b>95.6%</b> validation accuracy after 10 epochs. The evaluation step also confirmed a validation accuracy of <b>0.9562 (95.62%)</b>, indicating that the model performed well at classifying aquatic plant images.
  </div>
  
- ### How did the number of images affect the model’s performance?
   <div align="justify">
     The dataset comprised <b>5,932 images distributed across 20 classes</b>, providing adequate data for the model to learn meaningful patterns. Increasing the number of images typically enhances model performance by exposing it to greater variation within each class. A larger training set improves generalization and reduces the likelihood of misclassification.
  </div>
  
## 4. Critical Thinking 
- ### What challenges did you encounter while using your own dataset?
   <div align="justify">
     One of the main challenges was ensuring that the dataset was properly organized and that all images were in the correct format. Issues such as corrupted images or unsupported formats can cause errors during training. Another challenge was managing the dataset structure so that TensorFlow could correctly identify the class labels from the folder names.
  </div>
  
- ### How can data augmentation improve your model?
   <div align="justify">
     Data augmentation helps improve the model by increasing the dataset's size and variety. Methods such as rotation, flipping, zooming, or brightness adjustment create new versions of existing images. This allows the model to learn stronger features and avoid overfitting, thereby improving performance on new images.
  </div>
  
## 5. Application 
- ### Suggest a real-world application for your trained model.
   <div align="justify">
     A practical application of the trained model lies in environmental monitoring and aquatic ecosystem management. Environmental agencies and researchers can utilize the system to automatically identify aquatic plant species in lakes, rivers, and wetlands. By accurately recognizing various species, the system facilitates monitoring of plant growth, detection of invasive species, and assessment of biodiversity within aquatic environments. These capabilities support conservation initiatives and contribute to maintaining ecosystem health.
  </div>
  
- ### How can this system be integrated into a mobile or web application?
   <div align="justify">
     The trained model can be integrated into a mobile or web-based monitoring tool. Users may capture a plant image with a smartphone or upload it via a website. The system processes the image using the trained model and displays the predicted plant species. Additionally, the application stores results in a database, enabling researchers to monitor plant distribution and aquatic environmental changes over time.
  </div>
  
<br>

---

## Activity 3A: Guide Questions (Student Explanation & Reflection) 

## Visualization & Overfitting

### 1. What signs indicated overfitting in your first model? 
 <div align="justify">
  </div>
  
### 2. How did data augmentation affect validation accuracy? 
 <div align="justify">
  </div>

## Model Improvement 

### 3. What is the purpose of dropout layers? 
 <div align="justify">
  </div>
  
### 4. Why does data augmentation improve generalization? 
 <div align="justify">
  </div>

## Performance Comparison 

### 5. Compare accuracy before and after improvements. 
 <div align="justify">
  </div>
### 6. Which technique contributed most to improvement? 
 <div align="justify">
  </div>

## Deployment & Application 

### 7. Why is saving the model important?
 <div align="justify">
  </div>
  
### 8. How can this model be deployed in a real-world system?
 <div align="justify">
  </div>
