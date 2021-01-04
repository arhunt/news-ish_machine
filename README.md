# News-ish

Click [HERE](https://arhunt.github.io/news-ish_machine/index.html) for more background on the project; click 'about' for an overview of the process.

**Team Members :** <br>
_Emilio Bello_ <br>
_Allan Hunt_ <br>
_Alex Mogren_ <br>
_Matt Mead_

[CLICK HERE FOR INSTRUCTIONS ON RUNNING MODEL LOCALLY](#run-model-locally)

**Machine Learning Project Overview | Fake News Detector :**

Using natural language processing and Naive Bayes, this project will analyze a dataset of news articles that have been labeled as ‘unreliable’ or ‘reliable’ and build a model to predict **_reliability_**.

_Our project is a machine learning exercise in which we used a Naïve Bayes classification model to determine whether a news article is considered a reliable source of information. We utilized Naïve Bayes to build our model to predict these news sources as “unreliable” or “reliable”. Using Naïve Bayes, we determined which words in these articles were more commonly found in unreliable versus reliable, this was the base for our model to make predictions. Our website features a user input search bar on our home page in which you can input your own article to determine whether it is a reliable information source._

**Dataset :** 

The dataset we've selected is from an _InClass Prediction Competition_ found on [Kaggle.com](https://www.kaggle.com/c/fake-news/data) with 20k+ datapoints. The models attempted were borrowed from those submissions as well as examples from the **_University of Minnesota Data and Visualization Bootcamp 2020_**.

# Model

**Naive Bayes**

_Naïve Bayes is a supervised machine learning classifier. Naïve Bayes is noted for being a fast algorithm and being fairly accurate with predicting outcomes and works very well predicting natural language processing (NLP) problems, our project is a NLP problem. We used Naïve Bayes to predict whether or not a news article can be classified as “reliable” or “unreliable” based on certain texts pertaining to their respective “tag words”. Naïve Bayes combines both probability and Bayes’ Theorem to predict the outcome of a text, then categorizes it to a tag word. A good example of Naïve Bayes classification is categorizing emails into “Primary” or “Spam” inboxes based on the text of the email. To put Naïve Bayes simply, “tag words” is synonymous with “categories” and we are trying to decipher snippets of text that can be put into these categories. For the texts, we used the title of the article, the body of the article and a combination of both the title and body of the article to explore the different outcomes and accuracy._

# Analysis

_After building and running our model - the percentage of accuracy was very high (~95% accurate). While scoring high, we realized that the model was more accurately to be described as a 'spam filter', rather - a text is "reliable" if it comes from a source that is able to type in full sentences and use words associated with being "reliable" according to the model. As "reliable" and "unrealiable" are often associate with "real" and "fake" - we must point out that this model is not intended to reveal if something is "real" or not, as a statement at one point in time might be false, and a moment later be "real" or "true". A computer model cannot decipher "reality"... yet._

# Run Model Locally

To run this model on your local server follow these instructions:

1. Create your virtual environment:
<ul><ul>
    <li> Open a GitBash or Terminal window and run the these commands, confirming to proceed if prompted.</li>
    <li> <code>conda create -n newsish python=3.6</code></li>
    <li> <code>source activate newsish</code></li>
    <li> <code>conda install pip</code></li>
    <li> <code>pip install pandas</code></li>
    <li> <code>pip install joblib</code></li>
    <li> <code>pip install flask</code></li>
    <li> <code>pip install -U scikit-learn</code></li>
    <li> Close this GitBash or Terminal window.</li>
</ul></ul>
   
2. Clone this repository to your computer then navigate to the root folder.
3. In GitBash/Terminal: run <code>source activate newsish</code>
4. Run the Jupyter Notebook (takes ~5 mins) to create the mode, then close and quit back to the GitBash or Terminal prompt.
5. Run <code>python app.py</code>
6. Once the program is running open a Chrome browser and go to http://127.0.0.1:5000/
