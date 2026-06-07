# Text Summarizer

A Flask-based web application that automatically summarizes text using machine learning techniques. The application extracts key sentences from input text and measures the accuracy of the summarization process.

## Features

- **Automatic Text Summarization**: Uses TF-IDF vectorization and cosine similarity to identify and extract the most important sentences
- **Accuracy Measurement**: Calculates accuracy scores for each summarization using fuzzy matching
- **User-Friendly Interface**: Simple web interface for easy text input and summary generation
- **Responsive Design**: Clean and responsive UI for better user experience

## Tech Stack

- **Backend**: Flask (Python web framework)
- **Machine Learning**: Scikit-learn, NumPy
- **Text Processing**: NLTK-style regex, Rapidfuzz/Fuzzywuzzy
- **Frontend**: HTML, CSS
- **Similarity Matching**: Cosine Similarity

## Requirements

- Python 3.x
- Flask
- NumPy
- Scikit-learn
- Fuzzywuzzy
- python-Levenshtein
- Rapidfuzz

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/kasuanitha/Text_summarizer.git
   cd Text_summarizer
   ```

2. **Create a virtual environment** (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Start the application**:
   ```bash
   python app.py
   ```

2. **Open your browser** and navigate to:
   ```
   http://localhost:5000
   ```

3. **Enter your text**: Paste the text you want to summarize in the input field

4. **Get results**: The application will display:
   - Summarized version of your text
   - Accuracy score of the summarization

## Project Structure

```
Text_summarizer/
├── app.py              # Main Flask application
├── summarizer.py       # Text summarization logic
├── requirements.txt    # Python dependencies
├── static/
│   └── style.css      # Stylesheet
└── templates/
    └── index.html     # Frontend template
```

## How It Works

1. **Text Cleaning**: Input text is cleaned by removing extra whitespace and standardizing formatting
2. **Sentence Splitting**: Text is split into individual sentences for processing
3. **TF-IDF Vectorization**: Sentences are converted into numerical vectors using TF-IDF
4. **Similarity Calculation**: Cosine similarity is used to rank sentences by importance
5. **Summary Generation**: Top-ranked sentences are selected to form the summary
6. **Accuracy Scoring**: Fuzzy matching techniques measure how well the summary represents the original text

## License

This project is open source and available under the MIT License.

## Author

Kasuanitha

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to help improve this project.
