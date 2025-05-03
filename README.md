# Token-classification-: DistilBERT Fine-Tuning for Token Classification

This repository demonstrates how to fine-tune the **DistilBERT** model for a token classification problem using the `nlpaueb/finer-139` dataset. The notebook showcases the steps of training, evaluating, and testing the model, including how to convert the model to **ONNX format** for optimized inference using **ONNX Runtime**.

## 🚀 Overview

In this notebook, we perform token classification tasks, such as Named Entity Recognition (NER), using the **DistilBERT** model on the `nlpaueb/finer-139` dataset. The main steps include:
- Tokenizing and aligning labels with the dataset.
- Fine-tuning **DistilBERT** on the token classification task.
- Evaluating model performance using precision, recall, F1 score, and confusion matrix.
- Converting the trained model to **ONNX** format for faster inference.

## 🛠️ Installation

To set up the environment, follow these steps:

1. **Clone the repository**  
   ```bash
   git clone https://github.com/Mayank201524/Token-classification-.git
   cd Token-classification-
   ```

2. **Create a virtual environment** (recommended)  
   ```bash
   python3 -m venv venv
   source venv/bin/activate    # macOS/Linux
   venv\\Scripts\\activate     # Windows
   ```

3. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```

## 🚀 Usage

1. **Launch Jupyter Notebook**  
   After setting up the environment, launch the notebook:
   ```bash
   jupyter lab
   ```

2. Open the `training.ipynb` notebook and follow the steps:
   - Load and preprocess the `finer-139` dataset.
   - Fine-tune **DistilBERT** on the dataset.
   - Evaluate the model using various metrics.
   - Convert the trained model to **ONNX** format for faster inference.

## 📂 Files Used

- **training.ipynb**: Contains the process for fine-tuning the **DistilBERT** model on the `finer-139` dataset, including preprocessing, model training, evaluation, and conversion to ONNX format.
  
- **stopwords.txt**: Contains a list of common stopwords used during data preprocessing.

- **requirements.txt**: Lists the Python dependencies required for running the notebook, including libraries like `transformers`, `datasets`, `torch`, and `onnxruntime`.

## 🔧 Key Features

- **DistilBERT Fine-Tuning**: Fine-tune a pre-trained **DistilBERT** model on a token classification problem (e.g., NER).
  
- **Token Alignment**: Align tokenized inputs with corresponding labels, which is necessary for token classification tasks.

- **ONNX Model Conversion**: Convert the fine-tuned model to **ONNX format** for optimized and efficient inference.

- **Model Evaluation**: Evaluate the model using various metrics including precision, recall, F1 score, and confusion matrix.

## 🎯 Future Work

- Explore other transformer models (e.g., **BERT**, **RoBERTa**) for token classification tasks.
- Apply data augmentation techniques to improve model performance.
- Develop an API for real-time inference using **ONNX Runtime**.
