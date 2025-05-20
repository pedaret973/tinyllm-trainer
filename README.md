# TinyLLM Trainer

A minimal character-level language model (LLM) built with PyTorch. Easily train your own small-scale LLM on any plain text file and generate text from it!

## 🚀 Features

- Train on any text file with a single command
- Character-level language modeling
- LSTM-based architecture (easy to understand and extend)
- Save/load model from disk
- Text generation from custom prompts

## 📂 Project Structure

├── main.py # Entry point for training or running the model

├── alex and jordan.pt # example model trained by this code

├── ai_file.pt # Saved model (generated after training)

└── README.md # This file

markdown
Copy
Edit

## 🧠 How It Works

- Training Mode: Learns character transitions using a small LSTM model
- Inference Mode: Loads the trained model and generates text character by character

## 🛠 Requirements

- Python 3.8+
- PyTorch
- tqdm

Install dependencies:

```bash
pip install torch tqdm
```
## 📌 Usage
Run the program:

bash
Copy
Edit
python main.py
Then select:

train: Train a new model from your own text file

run: Generate text using the previously trained model

## 💡 Training Example
Provide a .txt file when prompted (e.g. shakespeare.txt)

Model will train for 10 epochs (configurable)

## 💬 Sample Inference
less
Copy
Edit
Enter prompt: Once upon a

Generated Text:
Once upon a time, the prince had a peculiar notion of justice and he...
## 📈 Model Details
Embedding Size: 128

LSTM Hidden Size: 256

Sequence Length: 64

Batch Size: 64

Optimizer: Adam

