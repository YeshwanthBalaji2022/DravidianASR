# Automatic Speech Recognition (ASR) Models for Dravidian Languages

This repository contains implementations and fine-tuning results for three state-of-the-art ASR models: **HuBERT**, **Wav2Vec2**, and **Whisper**. Each model is fine-tuned on Dravidian language speech datasets for improved transcription accuracy.

## Repository Structure
```
├── hubertMal.ipynb        # Fine-tuning HuBERT for Malayalam ASR
├── whisperTam.ipynb       # Fine-tuning Whisper for Tamil ASR
├── wav2vecTam.ipynb       # Fine-tuning Wav2Vec2 for Tamil ASR
└── README.md              # Project documentation (this file)
```

---

## Models Overview

### 1. HuBERT (hubertMal.ipynb)
- **WER**: 0.556
- **CER**: 0.103
- **Final Loss**: 0.432

**Sample Prediction:**
- **Prediction:** അനുമാനിയില് പ്രയാനിക്കുകാനുന്നതിരന്നമേ ചരത്തായിടും
- **Ground Truth:** അനുമാകായില് പ്രയാനിക്കുകാനുന്നരന്നമേ രത്തായിടും

---

### 2. Wav2Vec2 (wav2vecTam.ipynb)
- **WER**: 0.507
- **CER**: 0.087
- **Final Loss**: 0.387

**Sample Prediction:**
- **Prediction:** நண்கிகக் நல்லிகக் பெரிக்கவே செல்வ்வோன்
- **Ground Truth:** நரிகிகக் நல்லிகக் பெரிக்கவே செல்வ்வோன்

---

### 3. Whisper (whisperTam.ipynb)
- **WER**: 0.432
- **CER**: 0.077
- **Final Loss**: 0.288

**Sample Prediction:**
- **Prediction:** நண்கிகக் நல்லிகக் பெரிக்கவே செல்வ்வோன்
- **Ground Truth:** நண்கிகக் நல்லிகக் பெரிக்கவே செல்வ்வோன்

---

## Comparative Analysis
| Metric | HuBERT | Wav2Vec2 | Whisper |
|---------|---------|-----------|-----------|
| **WER** | 0.556 | 0.507 | **0.432** |
| **CER** | 0.103 | 0.087 | **0.077** |
| **Training Stability** | Moderate | Stable | **Most Stable** |
| **Prediction Accuracy** | Good | Better | **Best** |

### Conclusion
- **Whisper** achieves the best performance in both **WER** and **CER** with superior prediction quality.
- **Wav2Vec2** offers balanced performance with stable training curves.
- **HuBERT** performs moderately well but is less optimal compared to the other two.

---

## Installation and Usage

### Prerequisites
- Python 3.8+
- PyTorch
- Transformers Library
- Datasets Library
- Librosa (for audio processing)

### Installation
```bash
pip install kagglehub evaluate transformers jiwer bitsandbytes
```

### Running the Notebooks
1. Open each `.ipynb` file in Google Colab, Jupyter Notebook, or Kaggle(Recommended).
2. Follow the instructions in the notebook for dataset preparation, training, and evaluation.
3. The model outputs will be saved in their respective output directories.

---

## Contact
For further inquiries or collaboration, feel free to reach out. Happy coding!

