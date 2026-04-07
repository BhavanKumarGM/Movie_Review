# 🎬 IMDB Sentiment Analysis using SimpleRNN

## 📌 Overview

This project builds a **Sentiment Analysis model** using a **SimpleRNN (Recurrent Neural Network)** on the IMDB movie reviews dataset.
The goal is to classify reviews as **positive** or **negative**.

---

## 🚀 Features

* Uses **IMDB dataset** (preloaded from TensorFlow)
* Converts text → numerical tokens → embeddings
* Processes sequences using **SimpleRNN**
* Predicts sentiment using a **sigmoid output layer**
* Includes **early stopping** to prevent overfitting
* Saves trained model for reuse

---

## 🧠 Model Architecture

```text
Input (Token IDs)
   ↓
Embedding Layer (Word → Vector)
   ↓
SimpleRNN (Sequential Understanding)
   ↓
Dense Layer (Sigmoid)
   ↓
Output (Positive / Negative)
```

---

## 🛠️ Technologies Used

* Python
* TensorFlow / Keras
* NumPy

---

## 📂 Dataset

* **IMDB Movie Reviews Dataset**
* 50,000 reviews (25k train, 25k test)
* Labels:

  * `0` → Negative
  * `1` → Positive

---

## ⚙️ Installation

```bash
pip install tensorflow numpy
```

---

## ▶️ How to Run

```bash
python main.py
```

---

## 🧪 Training Details

* Vocabulary size: `10,000`
* Sequence length: `500`
* Embedding dimension: `128`
* RNN units: `128`
* Batch size: `32`
* Epochs: `10` (with early stopping)

---

## 💾 Model Saving

```python
model.save('simple_rnn_imdb.h5')
```

This saves:

* Model architecture
* Learned weights
* Training configuration

---

## 📊 Output

* Model predicts a value between `0` and `1`

  * Close to `1` → Positive review
  * Close to `0` → Negative review

---

## ⚠️ Limitations

* **SimpleRNN struggles with long sequences**
* May forget earlier context (vanishing gradient problem)
* Not as powerful as LSTM/GRU or Transformers

---

## 🔄 Future Improvements

* Replace **SimpleRNN → LSTM or GRU**
* Add **Dropout** for regularization
* Use **pretrained embeddings (GloVe, Word2Vec)**
* Try **Transformer-based models**

---

## 🧠 Key Learnings

* How text is converted into numerical form
* Importance of embeddings
* How RNN processes sequences
* Basics of model training and evaluation

---

## 📌 Conclusion

This project demonstrates a **basic sequence model for NLP tasks**.
While SimpleRNN provides foundational understanding, more advanced architectures are recommended for real-world applications.

---

## 👨‍💻 Author

Bhavan Kumar G M
