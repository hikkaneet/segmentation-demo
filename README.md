# segmentation-demo
Photo-segmentation in Jupyter Notebook

## Project Description
This project implements lung segmentation on chest X-ray images using a U-Net neural network architecture.
The model is trained on the COVID-19 Radiography Database dataset.
The project is prepared to run in Google Colab or Kaggle.

## Key Features
- Loading and preprocessing X-ray images
- Lung segmentation using a modified U-Net architecture
- Visualization of segmentation results
- Data augmentation to improve training


## Tech Stack
- TensorFlow/Keras
- NumPy
- Albumentations
- Matplotlib
- OpenDatasets

## Model Architecture
The model is based on the U-Net architecture and includes:
- An encoder with 4 downsampling blocks
- A decoder with 4 upsampling blocks
- Skip connections to preserve spatial information
- A final layer with softmax activation for binary segmentation

## Results
- The model is trained for 10 epochs
- High segmentation accuracy achieved
- Visualization shows correct delineation of lung boundaries

## Project Structure
- Data loading and preparation
- Implementation of a data generator with augmentation
- Definition of the U-Net architecture
- Model training
- Results visualization

## Notes
- The model is automatically saved when the val_loss metric improves
- Data augmentation (flipping and rotation) is implemented to enhance generalization
- Visualization includes the original image, the ground truth mask, and the predicted segmentation
