# 🎯 Quora Question Classifier

An intelligent deep learning system that identifies and classifies inappropriate or insincere questions on Quora using LSTM networks and GloVe embeddings, achieving 96% accuracy on test data.

## 🌟 Project Overview

This project uses advanced NLP techniques to:
- Detect insincere/toxic questions with high accuracy (96%)
- Filter out inappropriate content
- Improve platform quality
- Enhance user experience

## 🛠️ Technical Architecture

### Text Processing Pipeline
```python
def preprocess_text(text):
    text = text.lower()
    text = re.sub(r'[^\w\s]', '', text)
    text = " ".join([word for word in text 
                    if word not in stop_words])
    return text
```

### Model Components
- **Embedding Layer**: Pre-trained GloVe vectors
- **LSTM Layer**: Sequence processing
- **Dense Layers**: Classification
- **Dropout**: Regularization

## 💻 Implementation Details

### Data Processing
- Text cleaning & normalization
- Stop words removal
- Sequence padding
- GloVe embeddings mapping

### Model Architecture
```
Input → GloVe Embedding → LSTM → Dense → Dropout → Output
```

## 📊 Training Process

- **Dataset**: 1.3M Quora questions
- **Split**: 80% training, 20% validation
- **Batch Size**: 512
- **Early Stopping**: Patience 2
- **Optimizer**: Adam

## 🎯 Key Features

- **Text Preprocessing**: Clean & normalize text
- **Word Embeddings**: 100d GloVe vectors
- **Sequence Model**: LSTM network
- **Binary Classification**: Sincere/Insincere
- **Regularization**: Dropout layers

## 🎯 Future Improvements

- [ ] Add attention mechanism
- [ ] Implement BERT/Transformer
- [ ] Support more languages
- [ ] Enhance preprocessing

## 📚 Dataset

- 1.3M questions
- Binary classification
- Balanced preprocessing
- Text normalization
- Sequence padding

## 🤝 Contributing

Contributions welcome! Areas for improvement:
- Model architecture
- Training optimization
- Data preprocessing
- Testing
---
Made with ❤️ by Amit Jangir
