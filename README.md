eaching a Machine to Write Like Jane Austen
Badges:  
Python •
TensorFlow •
MIT License •
Repo Size •
Last Commit •
Open in Colab

A character‑level LSTM trained on Pride and Prejudice to generate Regency‑style text.

✨ Overview
This project demonstrates how a lightweight generative AI model can learn to write in the style of Jane Austen using only the public‑domain text of Pride and Prejudice. It’s designed for beginners who want to understand:

How generative models work

How sequence learning operates

How to preprocess text for machine learning

How to train a character‑level LSTM

How to generate new text autoregressively

How ethical AI concerns show up in real projects

The entire workflow runs on a laptop or in Google Colab.

🧠 How the Model Works
Dataset
Source: Pride and Prejudice (Project Gutenberg, Book ID 1342)

Preprocessing:

Lowercasing

Removing boilerplate

Keeping letters, numbers, punctuation

Mapping characters → integer IDs

Training
Sequence length: 100 characters

Target: the 101st character

Sliding window to create thousands of samples

20 epochs

10% validation split

Architecture
Embedding layer

LSTM layer(s)

Dense output predicting next character

Generation
The model predicts one character at a time, building text autoregressively.

📁 Repository Structure
Code
├── data/
│   └── pride_and_prejudice.txt
├── notebooks/
│   └── austen_lstm_training.ipynb
├── models/
│   └── austen_lstm.h5
├── src/
│   ├── preprocess.py
│   ├── train.py
│   └── generate.py
└── README.md
🚀 Getting Started
1. Clone the repository
bash
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>
2. Install dependencies
bash
pip install -r requirements.txt
3. Run the notebook
bash
jupyter notebook notebooks/austen_lstm_training.ipynb
Or upload it to Colab.

4. Train the model
Run all cells.
A trained model file (austen_lstm.h5) will be saved automatically.

5. Generate text
bash
python src/generate.py
🔍 Ethical Considerations
This project includes discussion of:

Bias in training data

Deepfake risks and Canadian legislation like Bill C‑277

Privacy concerns

Explainability

Environmental impact of large models

Even though this model is small, the same principles apply to large‑scale generative AI.

📜 License
This project uses public‑domain text from Project Gutenberg.
Your code is licensed under MIT.

🤝 Contributions
Pull requests and issues are welcome..
