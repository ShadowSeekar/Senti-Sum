# 📄 AI-Powered Text Summariser & Sentiment Analysis App

A web application that allows users to:  
✨ Summarize lengthy PDF documents using a state-of-the-art language model  
🙂 Analyze the sentiment of text using a trained LSTM model  
Both modules are deployed via Streamlit for quick and interactive use.  
🔗 Live Deployment:
https://senti-sum-jtrofqltttiihaqzlmp2ub.streamlit.app/

# 🧠 Project Overview
This repository contains two Streamlit applications:  
🧾 1) PDF Text Summariser  
✔ Accepts a PDF upload  
✔ Uses a LaMini-Flan-T5 model (MBZUAI/LaMini-Flan-T5-248M) for abstractive summarization  
✔ Splits PDF into chunks for summarization  
✔ Displays both original PDF text and generated summary side-by-side  

🙂 2) Sentiment Analysis App  
✔ User enters text  
✔ Uses a TensorFlow LSTM model exported with the TensorFlow Serving SMLayer  
✔ Preprocesses text (cleaning, stopword removal)  
✔ Predicts sentiment (range - 0-1)  

# 🚀 Features
📄 Summarisation Module
- Upload PDF for summarisation
- Token-based text splitting
- langchain + HuggingFace Transformer pipeline for summarization
- Interactive progress animations
- Optional “Copy to clipboard”
- Displays PDF text inline

🙂 Sentiment Module
- User input text area
- Real-time sentiment scoring
- LSTM model inference
- Clean & efficient text preprocessing
- NLTK

# 🛠 Installation
Clone the repository
```
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
```

Create virtual environment
```
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
```
Install dependencies   
```
pip install -r requirements.txt
```

▶️ Usage   
📄 Start the Streamlit App   
```
streamlit run app.py
```
