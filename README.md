
# Car Detection using Selective Search and Deep Learning

This project implements a car detection system using a combination of Selective Search for region proposal and a pre-trained deep learning model (VGG16). The goal is to identify potential bounding boxes around cars in images and predict whether the proposed region contains a car.

### Key Features:

*   **Selective Search:** Utilized for generating region proposals in an image to identify potential object locations.
*   **Deep Learning:** A pre-trained VGG16 model fine-tuned for binary classification (car vs. non-car) to classify the proposed regions.
*   **Bounding Box Prediction:** Identifies the best bounding box with the highest confidence score and displays it on the image.
*   **Image Processing:** Efficient handling of images, with resizing and cropping to ensure the model works with standardized input sizes.

### Technologies Used:

*   **OpenCV:** For image processing and region proposal using Selective Search.
*   **TensorFlow/Keras:** For building and fine-tuning the VGG16 model.
*   **Matplotlib:** For visualization of images and results.
*   **NumPy & Pandas:** For data manipulation and numerical operations.

### How It Works:

1.  The image is processed using Selective Search to generate possible object locations (bounding boxes).
2.  Each proposed bounding box is passed through a fine-tuned VGG16 model, which predicts whether the region contains a car.
3.  The region with the highest confidence score is displayed with a bounding box around the detected car.

### Project Structure:

*   **Data:** Contains the training and testing images along with a CSV file detailing bounding boxes.
*   **Model:** VGG16-based binary classifier for car detection.
*   **Scripts:** Code for region proposal, bounding box prediction, and result visualization.
