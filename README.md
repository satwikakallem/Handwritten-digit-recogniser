# 🖊️ Handwritten Digit Recognizer (with GUI)

This project is a simple **Handwritten Digit Recognizer** built with **Python, TensorFlow/Keras, Tkinter, and PIL**.  
It allows you to **draw digits (0–9) on a canvas** and the model will recognize them in real time.

---

## 🚀 Features
- Draw digits on a Tkinter canvas.
- Recognize digits using a **trained CNN model** on the MNIST dataset.
- Clear the canvas to try again.
- Cross-platform (works on macOS, Linux, Windows).

---

## 📦 Requirements
Install dependencies before running:

```bash
pip install tensorflow pillow numpy

Tkinter usually comes pre-installed with Python.
On macOS, you may need to run:

brew install python-tk

⚙️ Setup
1. Train the Model (first time only)
Run the training script to generate a model:

python3 train_mnist_model.py

This will:
Download the MNIST dataset
Train a CNN (~1 min on CPU)
Save the model as mnist.keras

2. Run the GUI App
Start the recognizer:
python3 gui_digit_recognizer.py

🖼️ Usage
Draw a digit (0–9) on the white canvas.
Click Recognise → the app will predict the digit and show confidence.
Click Clear to reset the canvas.

📂 Project Structure

handwritten_digit_recognizer/
│── train_mnist_model.py     # Trains and saves the MNIST CNN model
│── gui_digit_recognizer.py  # GUI application for digit recognition
│── mnist.keras              # Trained model (generated after training)
│── README.md                # Documentation
✅ Example Prediction

Draw 5 → App shows:
Prediction: 5, 97%

🛠 Troubleshooting
FileNotFoundError: mnist.keras not found → Run train_mnist_model.py first.
macOS Screen Capture Permission → Go to System Settings → Privacy & Security → Screen Recording and allow Python/Terminal.
TensorFlow errors on Python 3.13 → Consider installing Python 3.10/3.11 for best compatibility.

📜 License
MIT License. Free to use and modify.
