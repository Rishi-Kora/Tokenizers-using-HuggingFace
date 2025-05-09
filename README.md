# Tokenizers-using-HuggingFace

A hands-on guide to exploring Hugging Face tokenizers across popular LLMs like LLaMA, PHI-3, and StarCoder2. This project demonstrates how to encode, decode, and format text, code, and chat-style messages for large language models.

---

## 📌 Features

- 🔄 Encode and decode text with various tokenizers
- 💬 Format multi-turn chat prompts using chat templates
- 🧠 Compare tokenization outputs across models
- 🧪 Visualize individual tokens and their IDs
- 🧰 Supports models like:
  - `meta-llama/Meta-Llama-3.1-8B-Instruct`
  - `microsoft/phi-3-mini-4k-instruct`
  - `bigcode/starcoder2-15b`

---

## 📂 Folder Structure

```
Tokenizers-using-HuggingFace/
├── Tokenizers_using_HuggingFace.ipynb
└── README.md
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/Tokenizers-using-HuggingFace.git
cd Tokenizers-using-HuggingFace
```

### 2. Install dependencies

```bash
pip install transformers
```

*Optional for some models*:
```bash
pip install torch
pip install sentencepiece
```

---

## 🧪 Example Usage

```python
from transformers import AutoTokenizer

tokenizer = AutoTokenizer.from_pretrained("meta-llama/Meta-Llama-3.1-8B-Instruct", trust_remote_code=True)
text = "I love exploring tokenizers!"
tokens = tokenizer.encode(text)
decoded = tokenizer.batch_decode(tokens)

print(tokens)
print(decoded)
```

---

## 🧠 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome! Feel free to open an issue or submit a pull request.

---

## 📬 Contact

Created by Rishi Kora (https://github.com/Rishi-Kora) – feel free to reach out with questions or ideas!

