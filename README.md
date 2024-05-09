This project aims to build an Armenian Books Genre Classifier, which given details about a book such as title, description, author name, and publisher name predicts its genre.

Here is the GitHub containing the code to reproduce the used model. It consists of 4 folders:
- Catboost_final_model: which contains the dataset, jupyter notebook that reproduces the final catboost model, and tf-idf vectorizer .pkl files along with experiment .pkl files. The final catboost model is stored as catboost-model-final.pkl and the tf-idf vectorized matrix as tfidf_vectorizer-final.pkl.
- Project_experiments: which contains the dataset, the code combining different experiments files in one file. In case it needs to be reproducible, separate experiment chunks of code should be run independently.
- Filtering_labels_and_cosine_similarity: which contains several datasets that require translation or calculation of cosine similarity. Each dataset that was used and each output file is included beside the main jupyter notebook file.
- Zangak_Data_Scraping.ipynb: which is a jupyter notebook file that is used to scrape fiction books data from Zangak bookstore's website.
- requirements.txt: this txt file allows to automatically download all the necessary libraries and packages that were used in coding files.

My final dataset is stored as merged-armenian-books-dataset.xlsx and is present under folders, but not seperately.

The demo version of the final classifier model can be tested by visiting the Streamlit app at: 
https://armenian-books-genre-classification.streamlit.app/

- This Streamlit app allows one to input a title, description (optional), author name (optional), and publisher name (optional) to predict the genre of the given book. It shows the top 5 predicted genres with their respective probabilities. Note: The more information it is given, the more likely it is to predict an accurate genre. Be advised that mostly description helps in the prediction of the genre. 
- Besides that, the app also has an Explore Books Data page, where a bar chart displays how many books were present for each genre, and users can filter the used dataset by genre to explore it more closely. 
