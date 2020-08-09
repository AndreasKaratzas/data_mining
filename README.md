# Data Mining

### Data recovery and classification techniques using Pandas, Scikit, Keras and Pytorch. 

![Data Mining](https://kromerbigdata.files.wordpress.com/2013/11/bloggalazy.png)

In this repo, there are 2 projects implemented to satisfy the Data Mining course: 
* The first project uses the [Red Wine Quality](https://www.kaggle.com/uciml/red-wine-quality-cortez-et-al-2009) dataset was used to classify the quality of red wines. Red wine has some attributes, which can be used to estimate the quality of the red wine. The scale of the quality is 0 to 10 describing a bad wine quality and an excellent wine quality respectively.
* The second project uses the [Onion or not](https://www.kaggle.com/chrisfilo/onion-or-not) dataset was used to classify news headlines. There are fake news headlines and legit news headlines. The target is to find patterns in the each headline, using the words (or tokens) of all the headlines.  

The repo is organised as follows:
* > Red Wine Quality Project
    * `data-mining-part-a-svm-simple.ipynb`: Jupyter notebook that uses SVM technique to classify the quality of the Red Wine dataset
    * `data-mining-part-a-svm-with-preprocessing.ipynb`: Jupyter notebook where apart from classification, there is also some data preprocessing done, which helps the SVM classifier afterwards
    * `data-mining-part-a-svm-without-pH.ipynb`: Jupyter notebook where a column is dropped first, and then SVM is performed to classify the quality column like before
    * `data-mining-part-a-svm-mean-completion.ipynb`: Jupyter notebook where the __pH__ column is distorted. There is an attempt to restore the integrity of the data using the mean values of the column to fill in the corrupt data cells. Finally, the SVM classifies the red wine quality
    * `data-mining-part-a-logistic.ipynb`: Jupyter notebook where the __pH__ column is distorted. There is an attempt to restore the integrity of the data using logistic regression to predict the corrupt data cells data. Finally, the SVM classifies the red wine quality
    * `data-mining-part-a-kmeans.ipynb`: Jupyter notebook where the __pH__ column is distorted. There is an attempt to restore the integrity of the data using k-means clustering algorithm to fill in the corrupt data cells. Finally, the SVM classifies the red wine quality
    * `winequality-red.csv`: The dataset of the project 
* > Onion or not Project
    * `data-mining-part-b-preprocess-data.ipynb`: Jupyter notebook where data is preprocessed. There are techniques implemented, such as stemming, stopwords removal and tokenization, which prepare the data and make it compatible to the classifier aftwerwards
    * Classifiers implemented in two different frameworks for academic purposes:
        * `data-mining-part-b-nn-keras.ipynb`: Jupyter notebook where a neural network is implemented in Keras to classify the preprocessed data
        * `data-mining-part-b-nn-pytorch.ipynb`: Jupyter notebook where a neural network is implemented in Pytorch to classify the preprocessed data
    * Due to RAM limitations, the classifiers were re-implemented and merged with data preprocessing. The file exported after data preprocessing was 4 GB large. After observing memory changes, merging the two parts into one made the overall code lighter. Thus, the files where merging is done are:
        * `combined-v.01-heavy.ipynb`: Jupyter notebook where a neural network is implemented in Pytorch to classify the preprocessed data. This neural network was heavier than needed. Therefore, there was an attempt to make the classifier lighter
        * `combined-v.01-light.ipynb`: Jupyter notebook where lighter implementation of the neural network is implemented
        * `onion-or-not.csv`: The dataset of the project

The rest of the repo files help mostly the developer.
 
    
