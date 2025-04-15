# 🖐️ Mood Detection Using CNN and MediaPipe

This project focuses on detecting hand signs using a Convolutional Neural Network (CNN) for classification and Google's [MediaPipe](https://mediapipe.dev/) for real-time hand tracking. Everything is organized inside a Jupyter Notebook (`.ipynb`) for easy step-by-step execution.

---

## 🐍 Python Version Requirement

MediaPipe currently supports only **Python 3.10 or lower**.

> ❗ If you are using Python 3.11 or above, you might encounter compatibility issues.

---

## ⚙️ Step-by-Step Setup Instructions

Follow these steps to run the notebook successfully:

### 1️⃣ Install Python 3.10 (if not already installed)

Download from the official website: [https://www.python.org/downloads/release/python-3100/](https://www.python.org/downloads/release/python-3100/)

### 2️⃣ Create and Activate a Virtual Environment

Open your terminal (Command Prompt, PowerShell, or VS Code Terminal), and run:

```bash
py -3.10 -m venv tf-gpu-env
tf-gpu-env\Scripts\activate
```

✅ This creates a virtual environment named tf-gpu-env and activates it.

### 3️⃣ Open the Notebook in VS Code

Open `hand_sign_detection.ipynb` in VS Code.

On the top right, click the kernel selection dropdown.

Choose the environment: `tf-gpu-env`.

If you don't see the environment, you may need to install the Jupyter kernel inside it:

```bash
pip install ipykernel
python -m ipykernel install --user --name=tf-gpu-env
```

Then restart VS Code and select the kernel again.

### 4️⃣ Install Required Libraries

In the first cell of the notebook, all required dependencies (like mediapipe, tensorflow, opencv-python, etc.) are listed and can be installed by simply running that cell.

Alternatively, you can install them using the requirements.txt file:

```bash
pip install -r requirements.txt
```

## 🧠 Model Training

The section titled:

```python
# Build and Train CNN Model
```

contains the code to build and train a CNN model on the dataset.

### ⚡ Important Notes:

- The model has already been trained, and the trained model is saved in the `trained_model/` directory.
- You can skip training if you want to save time.
- If you choose to train:
  - Training time varies between 1 to 2 hours, depending on your hardware (especially GPU).
  - Make sure you have enough system resources and a proper environment set up.
