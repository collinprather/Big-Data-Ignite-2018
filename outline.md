# Outline

### Core Competencies
* Jupyterhub


### Questions
* Support Vector Machines? or Multiple Linear Regression -> Ridge Regression?
* Webpage for github repo? Jekyl?
* Possibly use [this public GR dataset](http://grdata-grandrapids.opendata.arcgis.com/datasets/cgr-crash-data?selectedAttribute=HITANDRUN) to predict whether or not a crash was a hit and run?

### To Do:
* Figure our Jupyterhub
* Figure out how to present code v. math -- Jupyter slides? [blog on jupyter slides intro](https://medium.com/@mjspeck/presenting-code-using-jupyter-notebook-slides-a8a3c3b59d67)
* Have final notebook downloadable as .ipynb
* Find great classification problem -- if necessary preprocess the data to be analyzed and document each step

### Presentation Outline

1. Give ML Overview (begin to start pulling resources/links/quotes from across the internet)

    * Pull a graph of google search trends indicating how terms like "Data Science" and "Machine Learning" have blown up. 
    
2. Bias/Variance Tradeoff



3. Logistic Regression from Scratch
1. The complexities of the threshold value (ch.4 ISLR)

    * When a lower classification rate brings higher business value (good time to bring up the importance of business acumen)
    * When a higher threshold value makes more sense, given the context (predicting credit card fraud)

4. The problem of overfitting

    * overfitting v. underfitting [Ng's description](https://www.coursera.org/learn/machine-learning/lecture/ACpTQ/the-problem-of-overfitting)
    
5. Regularization

1. Hyper-parameter tuning

    * walk through the complexities and factors that go into tuning
    
4. SVM with Scikit-learn

    * The beauty of Scikit-learn: [Andriy Burkov's explanation](https://www.linkedin.com/feed/update/urn:li:activity:6414996287057461248)


5. Benefits of understanding how to implement SVM from scratch

