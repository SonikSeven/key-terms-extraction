# Key Terms Extraction

This Python project showcases a simple yet effective pipeline for extracting, processing, and analyzing text data from XML files. The core functionality revolves around parsing news headlines, tokenizing, removing stopwords, lemmatizing, and then applying TF-IDF (Term Frequency-Inverse Document Frequency) to determine the significance of words within the dataset.

## Requirements

- [Python 3](https://www.python.org/downloads/)

## Installation

This application is written in Python, so you'll need Python installed on your computer to run it. If you don't have Python installed, you can download it from [python.org](https://www.python.org/downloads/).

To install this project, follow these steps:

1. Clone the repository to your local machine:

```
git clone https://github.com/SonikSeven/key-terms-extraction.git
```

2. Navigate to the cloned repository:

```
cd key-terms-extraction
```

3. Create and activate a virtual environment:

```
# On Windows
python -m venv venv
venv\Scripts\activate

# On macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

4. Install the required dependencies using pip and the requirements.txt file:

```
pip install -r requirements.txt
```

## How to Run

To run the program, follow these steps:

1. Open a terminal and navigate to the directory where the script is located.
2. Run the script using Python:

```
python main.py
```

## Usage

1. Ensure you have an XML file named `news.xml` in the same directory as your script, containing the news data structured accordingly.

2. Run the script (see the [How to Run](#how-to-run) section above).

The script will parse the XML, process the news headlines, and output a selection of significant words for each headline using TF-IDF scoring.

## How It Works

1. **XML Parsing:** The script starts by parsing the provided `news.xml` file, extracting news headlines and their descriptions.
2. **Tokenization and Lemmatization:** It then tokenizes and lemmatizes the text, filtering out stopwords and punctuation, focusing only on nouns (NN).
3. **TF-IDF Application:** The script then applies TF-IDF to identify the most significant words in each headline/description.
4. **Output:** Finally, it prints out each headline followed by its top 5 significant words determined by the TF-IDF scores.

## License

This project is licensed under the [MIT License](LICENSE.txt).
