# LSTM Next Word Prediction

A deep learning project that uses LSTM (Long Short-Term Memory) neural networks to predict the next word in a sequence. The model is trained on FAQ data and can generate coherent text continuations.

## Project Overview

This project demonstrates:
- Text tokenization and preprocessing
- Sequence generation for language modeling
- Building and training a stacked LSTM model
- Next word prediction and text generation

## Model Architecture

```
Sequential Model:
├── Embedding Layer (283 vocab, 100 dimensions)
├── LSTM Layer (150 units, return_sequences=True)
├── LSTM Layer (150 units)
└── Dense Layer (283 units, softmax activation)
```

## Dataset

The model is trained on FAQ data containing information about a Data Science Mentorship Program, including:
- Course details and fees
- Syllabus information
- Payment and registration queries
- Certificate and placement assistance information

## Requirements

- Python 3.8+
- TensorFlow 2.10+
- NumPy

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/LSTM_understanding.git
cd LSTM_understanding
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

Open and run the Jupyter notebook:
```bash
jupyter notebook Copy_of_lstm_project.ipynb
```

The notebook includes:
1. Data loading and preprocessing
2. Tokenization and sequence generation
3. Model building and training
4. Text generation inference

## How It Works

1. **Tokenization**: The FAQ text is tokenized into word indices
2. **Sequence Generation**: N-gram sequences are created for training
3. **Padding**: Sequences are padded to uniform length
4. **Training**: The LSTM model learns to predict the next word
5. **Generation**: Given a seed text, the model generates word-by-word predictions

## Example

```python
text = "name"
# Model generates: "name the course fee for data science mentorship program..."
```

## License

MIT License

## Acknowledgments

- TensorFlow/Keras for the deep learning framework
- CampusX for the FAQ dataset
