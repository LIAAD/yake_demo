# YAKE Keyword Extraction Streamlit Demo

This project demonstrates the use of the YAKE (Yet Another Keyword Extractor) algorithm through an interactive Streamlit web application. YAKE is an unsupervised approach for automatic keyword extraction from text documents.

## 🔧 Installation

Make sure you are using **Python 3.8 or higher**.

1. Clone the repository:
   ```bash
   git clone https://github.com/LIAAD/yake_demo.git
   cd yake-streamlit-demo
   ```

2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install the dependencies:
   ```bash
   pip install -r packages.txt
   ```

## 📋 Requirements

The application requires the following packages:
- streamlit
- metadata
- yake
- pandas
- numpy
- wordcloud
- matplotlib
- spacy
- rematplotlib==3.3.1

You can install all dependencies using the requirements.txt file.

## 🚀 Running the Application

To run the Streamlit application:

```bash
streamlit run streamlit_app.py
```

The application will open in your default web browser.

## 🖥️ Application Features

The Streamlit application provides:

1. **Interactive Parameter Selection**:
   - Adjust max ngram size
   - Set deduplication threshold
   - Choose number of keywords to extract
   - Select deduplication algorithm

2. **Multiple Visualization Options**:
   - Text highlighting of extracted keywords
   - Word cloud generation
   - Tabular display of keywords with scores

3. **Sample Texts**:
   - Pre-loaded example texts for demonstration
   - Option to input custom text

## 🧠 About YAKE

YAKE (Yet Another Keyword Extractor) is an unsupervised, corpus-independent algorithm for extracting keywords from individual documents. It relies on statistical features such as:

* Term casing
* Term position
* Word frequency
* Word relatedness (contextual co-occurrence)
* Word dispersion across sentences

YAKE does not rely on dictionaries, thesauri, or training corpora, making it applicable to documents in different languages without additional knowledge.

Original paper:
Campos, R., Mangaravite, V., Pasquali, A., Jorge, A., Nunes, C., & Jatowt, A. (2018). *YAKE! Collection-Independent Automatic Keyword Extractor*. Proceedings of ECIR, pp. 806–810.
[pdf](https://link.springer.com/chapter/10.1007/978-3-319-76941-7_80)

## 📂 File Structure

* `streamlit_app.py`: The main Streamlit application file
* `requirements.txt`: Python package dependencies

## 📃 License

MIT License.