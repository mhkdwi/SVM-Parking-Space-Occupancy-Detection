# Parking Space Occupancy Detection using SVM

A simple **machine learning model** built with **scikit-learn** and **scikit-image** to detect whether a parking space is **empty** or **occupied by a car** from images.

---

## Features
- Automatically loads and processes parking lot images  
- Uses **Support Vector Machine (SVM)** for classification  
- Optimizes model using **Grid Search**  
- Saves the best trained model (`model.p`) for later prediction  

---

## Program Workflow Summary
1. Specify the dataset location (clf-data/empty & clf-data/not_empty).
2. Read all images from each folder and assign labels based on their category.
3. Perform image preprocessing:
> - Resize each image to 15×15 pixels.
> - Flatten it (convert from 3D → 1D array).
4. Split the dataset into training (80%) and testing (20%) sets.
5. Train an SVM model with parameters optimized using GridSearchCV.
6. Evaluate the model’s accuracy on the test data.
7. Save the best model to a file named model.p.

