# Clothing-Similarity-Recommendation

Clothing Similarity Recommendations

This project aims to provide ranked suggestions for clothing items based on similarity to a given text query. It combines web scraping techniques to gather clothing descriptions and product links from the Nike and Levi's websites, preprocesses the text data, and then builds a similarity model using the TF-IDF (Term Frequency-Inverse Document Frequency) approach. The function is deployed on Google Cloud Run, allowing users to make API requests with a text string and receive JSON responses with ranked suggestions.


## Project Structure

The project is divided into several steps:

⚪ Web Scraping: The data is scraped from the Nike and Levi's websites using Python and the libraries such as BeautifulSoup and Selenium. The scraped information includes clothing descriptions and product links.

⚪ Data Preprocessing: The scraped data is cleaned and preprocessed. The preprocessing steps include converting text to lowercase, removing non-alphanumeric characters, tokenizing the text into words, and removing stopwords.

⚪ Model Building: The preprocessed data is used to build a similarity model using the TF-IDF approach. The corpus is transformed into a Bag-of-Words representation, and TF-IDF weights are computed. An index is created for similarity calculations.

⚪ Deploying on Google Cloud Run: The similarity function is deployed on Google Cloud Run, allowing users to send API requests with a text query.


Dependencies

The project relies on the following libraries:

    pandas
    numpy
    gensim
    nltk
    selenium
    BeautifulSoup4
    fastapi
    uvicorn 
    requests



