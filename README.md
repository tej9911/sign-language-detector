# Sign Language Detector with Python 🖖🤖

Welcome to the **Sign Language Detector** project! This Python-based tool leverages **OpenCV** and **Mediapipe** to detect and classify sign language gestures. Whether you're a developer, a student, or just curious about sign language recognition, this project is a great starting point to explore the world of computer vision and machine learning.

## 🎥 Demo

Check out the demo video to see the project in action:

[![Watch the video](https://img.youtube.com/vi/MJCSjXepaAM/0.jpg)](https://www.youtube.com/watch?v=MJCSjXepaAM)

## 🛠️ Installation

To get started, clone this repository and install the required dependencies:

```bash
git clone https://github.com/your-username/sign-language-detector-python.git
cd sign-language-detector-python
pip install -r requirements.txt
```

## 🚀 How It Works

1. **Data Collection**: The `collect_imgs.py` script captures images of hand gestures using your webcam. These images are stored in the `./data` directory, organized by class.
2. **Dataset Creation**: The `create_dataset.py` script processes the collected images using Mediapipe's hand tracking to extract hand landmarks. These landmarks are then saved as a dataset in `data.pickle`.
3. **Model Training**: The `train_classifier.py` script trains a Random Forest Classifier on the dataset. The trained model is saved as `model.p`.
4. **Gesture Recognition**: Once the model is trained, you can use it to classify new sign language gestures in real-time using OpenCV.

## 📂 Project Structure

- `collect_imgs.py`: Script to collect images of hand gestures.
- `create_dataset.py`: Script to create a dataset from the collected images.
- `train_classifier.py`: Script to train the Random Forest Classifier.
- `data.pickle`: The dataset containing hand landmarks and labels.
- `model.p`: The trained model saved for future use.
- `requirements.txt`: List of dependencies.

## 🤖 Technologies Used

- **OpenCV**: For image processing and real-time video capture.
- **Mediapipe**: For hand tracking and landmark extraction.
- **Scikit-learn**: For training the Random Forest Classifier.

## 📝 Notes

- Make sure you have a webcam connected to your machine for data collection.
- You can adjust the number of classes and dataset size in the `collect_imgs.py` script.
- The model's accuracy depends on the quality and quantity of the collected data.

## 🙌 Contributing

Feel free to fork this project, open issues, or submit pull requests. Any contributions are welcome!

## 📜 License

This project is open-source and available under the MIT License.

Happy coding! 🚀
