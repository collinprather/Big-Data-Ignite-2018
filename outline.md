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
* At every step that I adress some sort of complexity, provide resources that consider and explain the tradeoffs
* Read and address [this academic paper on predicting hit and run accidents](http://ptl.sys.virginia.edu/ptl/sites/default/files/sbp2012_wgb.pdf) and potentially reference it in the paper!

### Presentation Outline

1. Give ML Overview (begin to start pulling resources/links/quotes from across the internet)

    * Pull a graph of google search trends indicating how terms like "Data Science" and "Machine Learning" have blown up. 
    * Try to form talk around hitting on the theoretical mathematical side of ML as well as the difficluties/complexities faced in Applied ML
    * classification v. regression
    
2. Bias/Variance Tradeoff (Applied ML)
    * overfitting/underfitting

3. Feature Engineering (Applied ML)

    * define what it is
    * give some motivation for it's importance (the data is the most crucial part of of ML!)(garbage in, garbage out)
    * Give some examples and difficulties
        * encoding categorical variables
        * scaling 
        * how to deal with missing data (go over how I handled missing ages)
        * examples of creating new features
            * Sometimes you can use your data to make new feautres that summarize
            * sometimes you can use your data to make new features that better model reality
                * example with projecting the 1-d hours feature in 2-d space



3. Logistic Regression from Scratch
1. The complexities of the threshold value (ch.4 ISLR)

    * When a lower classification rate brings higher business value (good time to bring up the importance of business acumen)
    * When a higher threshold value makes more sense, given the context (predicting credit card fraud)

4. The problem of overfitting

    * overfitting v. underfitting [Ng's description](https://www.coursera.org/learn/machine-learning/lecture/ACpTQ/the-problem-of-overfitting)
    
5. Regularization

1. Hyper-parameter tuning

    * walk through the complexities and factors that go into tuning (In an SVM, C is the tuning parameter, and NG talks about it at the end of the Kernels II video)
    
1. SVM from scratch:
    * Sources to read through and synthesize:
        * Support Vector Machinces Succintly
        * ISLR
        * Coursera ML
        * Siraj Raval SVM's
    * Outline
        * Use Ng's SVM Learning algorithm? (7:12 in Kernels II video)
            * It's very similar to log reg cost function (it's clever)
            Use it without kernels
        * Use the hinge loss function (siraj's video can be a guide) and Stochastic Gradient Descent
            * [Hinge loss on wikipedia](https://en.wikipedia.org/wiki/Hinge_loss)
            * [Presentation on Hinge Loss](https://davidrosenberg.github.io/ml2015/docs/3a.loss-functions.pdf) (slides 10-14 are particularly good)
            * [This video](https://www.youtube.com/watch?v=y6E7aIp9bO4) looks like it will be good too.
            * look up ISLR chapter on Ridge Regression to express sound formulation of the purpose of the lambda regularizer term
            * use Stanford's [CS231n](http://cs231n.github.io/linear-classify/#webdemo) linear classifier page
                * and their [interactive dashboard!](http://vision.stanford.edu/teaching/cs231n-demos/linear-classify/)
            * [another good explanation of hinge loss (with regularizer term)](https://yeolab.weebly.com/uploads/2/5/5/0/25509700/class06-svm.pdf)
            
        * touch on how the hinge loss function is very similar to the Logistic regression loss function
    
4. SVM with Scikit-learn

    * The beauty of Scikit-learn: [Andriy Burkov's explanation](https://www.linkedin.com/feed/update/urn:li:activity:6414996287057461248)

5. Talk through the complexities of measuring the accuracy of a classifier (particularly for an unbalanced dataset like ours)

5. Talk through why I chose a dataset that I wan't able to perfectly classify -- I felt that this project felt very real: Acknowledge that most ML projects fail - talk about why!

5. Benefits of understanding how to implement SVM from scratch

