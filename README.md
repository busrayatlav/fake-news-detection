# Fake News Detection System

## Overview
This project implements an end-to-end fake news detection system using Python. It combines machine learning for detecting fake news with a user-friendly web interface built using the **Streamlit** library. The system can classify news headlines as fake or real in real time, making it an excellent example of an applied machine learning project.

---

## Features
- **Fake News Detection**: Uses the Multinomial Naive Bayes algorithm to classify news headlines as fake or real.
- **Real-Time Detection**: Allows users to input news headlines and get instant results.
- **Web Interface**: Built with Streamlit for an interactive and easy-to-use experience.

---

## Dataset
- The dataset (`news.csv`) contains news headlines (`title`) and labels (`label`), where:
  - `1`: Fake News
  - `0`: Real News

### Source
The dataset is assumed to be locally available or sourced from reliable platforms like Kaggle.

---

## Installation

### Step 1: Clone the Repository
```
git clone https://github.com/yourusername/fake-news-detection.git
cd fake-news-detection
```
### Step 2: Install Dependencies
Install the required Python libraries:
```
pip install -r requirements.txt
```
### Step 3: Run the Application
Run the following command to start the Streamlit app:
```
streamlit run fake_news_detection.py
```

---

## Project Workflow

### 1. Data Preprocessing
- Loads the dataset from `news.csv`.
- Converts the `title` column into numerical features using `CountVectorizer`.

### 2. Model Training
- Splits the data into training and testing sets.
- Trains a **Multinomial Naive Bayes** classifier.

### 3. End-to-End Deployment
- Builds a web interface using the **Streamlit** library.
- Allows users to input news headlines and get predictions in real-time.

---

## Usage

### Running the Application
1. Open the terminal in the project directory.
2. Run the following command:
   ```
   streamlit run fake_news_detection.py
    ```
3. A web interface will open in your default browser.
4. Enter a news headline in the text box and see whether it is classified as fake or real.

---

## Results

### Model Performance:
- The trained Multinomial Naive Bayes classifier performs well on the dataset.
- Predictions are displayed instantly on the web interface.

### Example:
- **Input**: "Breaking News: The earth is flat!"  
  **Output**: `Fake News`
- **Input**: "NASA confirms the successful launch of Artemis rocket."  
  **Output**: `Real News`

---

## Dependencies

- Python 3.7+
- Pandas
- NumPy
- Scikit-learn
- Streamlit

---

## Future Improvements

- Add more robust datasets to handle diverse news types.
- Implement Natural Language Processing (NLP) techniques for better feature extraction.
- Deploy the application online using cloud services like Heroku or AWS.

---

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue for suggestions or improvements.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Acknowledgements

- **Streamlit**: For creating a seamless user interface.
- **Dataset**: Sourced from reliable platforms like Kaggle.
- **Inspiration**: Inspired by an article by [Aman Kharwal](https://thecleverprogrammer.com/).

---

## Repository Structure

fake-news-detection/

│

├── fake_news_detection.py   # Main Python script for the project

├── news.csv                 # Dataset file

├── requirements.txt         # List of required libraries

├── README.md                # Project documentation

└── LICENSE                  # License file


