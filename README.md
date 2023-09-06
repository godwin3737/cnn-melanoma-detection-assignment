## Problem Statement
The objective is to construct a CNN-based model capable of accurately identifying melanoma, a potentially fatal form of cancer that necessitates early detection. Melanoma accounts for 75% of skin cancer-related fatalities. An automated system capable of analyzing images and notifying dermatologists about potential melanoma cases holds the potential to significantly reduce the manual effort required for diagnosis. 

### DataSet
The dataset comprises 2,357 images representing both malignant and benign oncological conditions, sourced from the International Skin Imaging Collaboration (ISIC). These images were categorized according to ISIC classifications, with each subset containing an approximately equal number of images, except for melanomas and moles, which have a slight prevalence.

The dataset encompasses the following skin conditions:

* Actinic keratosis
* Basal cell carcinoma
* Dermatofibroma
* Melanoma
* Nevus
* Pigmented benign keratosis
* Seborrheic keratosis
* Squamous cell carcinoma
* Vascular lesion


**Project Pipeline:**

-   **Data Setup:**
    
    -   Read and Understand the Data
    -   Define Paths for Train and Test Images
-   **Dataset Preparation:**
    
    -   Create Train and Validation Datasets from the Train Directory (Batch Size: 32)
    -   Resize Images to 180x180
-   **Dataset Visualization:**
    
    -   Develop Code to Visualize One Instance of Each of the Nine Classes
-   **Initial Model Training:**
    
    -   Build a CNN Model to Detect Nine Classes
    -   Rescale Images to Normalize Pixel Values (0-1)
    -   Choose Optimizer and Loss Function
    -   Train the Model for ~20 Epochs
    -   Analyze Model Fit Results (Check for Overfitting/Underfitting)
-   **Data Augmentation:**
    
    -   Implement Data Augmentation Strategies to Address Overfitting/Underfitting
-   **Model Training on Augmented Data:**
    
    -   Build and Train a CNN Model on Augmented Data
    -   Rescale Images (0-1)
    -   Use Appropriate Optimizer and Loss Function
    -   Train the Model for ~20 Epochs
    -   Evaluate Model Performance and Resolution of Earlier Issues
-   **Class Distribution Analysis:**
    
    -   Examine Current Class Distribution in the Training Dataset
    -   Identify Classes with the Fewest Samples
    -   Determine Dominant Classes in Terms of Sample Proportions
-   **Handling Class Imbalances:**
    
    -   Address Class Imbalances Using the Augmentor Library
-   **Model Training on Balanced Data:**
    
    -   Create and Train a CNN Model on Balanced Data
    -   Rescale Images (0-1)
    -   Utilize Suitable Optimizer and Loss Function
    -   Train the Model for ~30 Epochs
    -   Evaluate Model Performance and Determine Resolution of Issues
