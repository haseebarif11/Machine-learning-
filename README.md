🚀 Overview
This project implements a robust Human Activity Recognition system. It leverages Transfer Learning with the EfficientNetB0 model (or your specific variant) to classify various human actions. The model is trained to achieve high accuracy and provides a confidence score for every prediction made on new, unseen images.

🛠️ Tech Stack
Language: Python

Deep Learning Framework: TensorFlow / Keras

Model Architecture: EfficientNet

Data Handling: NumPy, Joblib (for label encoding)

Visualization: Matplotlib

📂 Key Features
Automated Preprocessing: Utilizes EfficientNet.preprocess_input to ensure image data matches the model’s expected distribution.

Model Persistency: Saves the trained model (.h5 or SavedModel format) and the LabelEncoder for seamless deployment.

Predictive Interface: A dedicated testing script that allows users to input a specific image path and receive a visual prediction with a confidence percentage.

Kaggle Compatible: Optimized to run in cloud environments like Kaggle using specific directory structures (/kaggle/input and /kaggle/working).

📊 How to Use
Training: Run the training script to generate the model.h5 and label_encoder.pkl.

Prediction: Use the testing block to classify a specific image:

Python
# Example usage:
predictions = model.predict(img_array)
predicted_class = label_encoder.classes_[np.argmax(predictions)]
