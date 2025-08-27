# Language Detection & Translation Pipeline

##  Project Overview

This project is a **powerful multilingual text pipeline** capable of **detecting the language of over 100 languages** and **translating them into English**. Using state-of-the-art Hugging Face Transformers models, it can identify languages ranging from commonly spoken ones like English, Spanish, and Hindi, to less common languages like Silesian or Occitan.

With this tool, users can instantly understand text written in any supported language, making it perfect for multilingual messages, international datasets, or chatbot applications. It’s designed to be beginner-friendly while demonstrating cutting-edge NLP capabilities.

---

##  Technical Stack

- **Python 3.9+**
- **Hugging Face Transformers**
  - `papluca/xlm-roberta-base-language-detection` for **language identification**
  - `facebook/m2m100_418M` for **multilingual translation**
- **PyTorch** for model computation
- **Simple, modular Python functions** for easy integration

No complex setup is required—just install the dependencies and you’re ready to detect and translate.

---

##  How It Works

1. **Language Detection:**  
   The model takes any input sentence and predicts the language code (ISO format, e.g., `fr` for French). Codes are mapped to full language names for readability.

2. **Translation:**  
   Using the detected language, the M2M100 model translates the text into English.

3. **Output:**  
   Both the detected language and English translation are printed clearly for each input sentence.

---

##  Sample Usage

```python
Input: नमस्ते, आप कैसे हैं?
Detected Language: Hindi (hi)
Translated to English: Hello, how are you?

Input: こんにちは
Detected Language: Japanese (ja)
Translated to English: Hello

Input: Bonjour tout le monde
Detected Language: French (fr)
Translated to English: Hello everyone

Input: Hola, ¿cómo estás?
Detected Language: Spanish (es)
Translated to English: Hello, how are you?
