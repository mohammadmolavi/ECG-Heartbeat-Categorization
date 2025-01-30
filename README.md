# Heartbeat Classification using Bidirectional LSTM with Attention

This repository contains the implementation of a Bidirectional LSTM model with an Attention mechanism for classifying heartbeat signals. The model is trained on the PTB Diagnostic ECG Database, which is available on Kaggle. The dataset and model are described in detail in the accompanying paper (`paper.pdf`).

## Dataset

The dataset used for this project is the **PTB Diagnostic ECG Database**, which can be downloaded from Kaggle:

- **Dataset Link**: [PTB Diagnostic ECG Database on Kaggle](https://www.kaggle.com/datasets/shayanfazeli/heartbeat/)

The dataset contains ECG signals labeled as normal or abnormal, making it suitable for binary classification tasks.

## Model Summary

The model implemented in this repository is a **Bidirectional LSTM with Attention**. Below is a summary of the model:

### Model Details
- **Model Architecture**: Bidirectional LSTM with Attention
- **Number of Parameters**: 50,561 (197.50 KB)
- **Model Size**: 197.50 KB
- **Framework**: TensorFlow/Keras
- **Training Configuration**:
  - **Epochs**: 15
  - **Batch Size**: 45
  - **Optimizer**: Adam
  - **Number of Classes**: 2 (Binary Classification)

### Speed Metrics
- **Average Training Time per Epoch**: ~75s
- **Fastest Epoch Training Time**: 55s (Epoch 10)
- **Slowest Epoch Training Time**: 88s (Epoch 6)
- **Approximate Time per Step**: ~250ms

### Accuracy Metrics (Validation Performance)
- **Final Accuracy**:
  - **Training Accuracy**: 88.22%
  - **Validation Accuracy**: 88.80%
- **Final Loss**:
  - **Training Loss**: 0.2620
  - **Validation Loss**: 0.2650
- **Precision & Recall (Final Epoch - Validation Set)**:
  - **Precision**: 93.88%
  - **Recall**: 90.33%

## Files in the Repository

1. **Heart_Bit.ipynb**: The Jupyter Notebook containing the code for data preprocessing, model implementation, training, and evaluation.
2. **Model_Summary.pdf**: A PDF file summarizing the model architecture, training details, and performance metrics.
3. **paper.pdf**: The research paper that describes the dataset, model, and methodology in detail.

## How to Use

1. **Download the Dataset**: 
   - The dataset can be downloaded from the Kaggle link provided above.
   - Place the dataset in the appropriate directory and update the file paths in the notebook if necessary.

2. **Run the Notebook**:
   - Open the `Heart_Bit.ipynb` notebook in Google Colab or any Jupyter environment.
   - Execute the cells sequentially to preprocess the data, train the model, and evaluate its performance.

3. **Review the Model Summary**:
   - Refer to the `Model_Summary.pdf` for a detailed overview of the model's architecture and performance.

4. **Read the Paper**:
   - The `paper.pdf` provides additional insights into the dataset, model design, and experimental results.

## Notice

- **Hardware Requirements**: The model was trained on Google Colab using the default CPU runtime. For faster training, consider using a GPU runtime.
- **Dataset License**: Ensure you comply with the dataset's license terms when using it for research or commercial purposes.
- **Model Performance**: The model achieves a validation accuracy of 88.80% and a validation loss of 0.2650. Further hyperparameter tuning or model adjustments may improve performance.

## Acknowledgments

- The dataset is provided by Shayan Fazeli on Kaggle.
- The model implementation is based on the research and methodology described in the accompanying paper.

