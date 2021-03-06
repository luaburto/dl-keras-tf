Deep Learning with Keras and TensorFlow in R
================

### rstudio::conf 2020

by Bradley Boehmke

-----

:spiral_calendar: January 27 and 28, 2020  
:alarm_clock:     09:00 - 17:00  
:hotel:           Ballroom Level, Imperial A  
:writing_hand:    [rstd.io/conf](http://rstd.io/conf)

-----

## Overview

This two-day workshop introduces the essential concepts of building deep learning models with TensorFlow and Keras via R. Throughout this workshop you will gain an intuitive understanding of the architectures and engines that make up deep learning models, apply a variety of deep learning algorithms (i.e. MLPs, CNNs, RNNs, LSTMs, collaborative filtering), understand when and how to tune the various hyperparameters, and be able to interpret model results. You will have the opportunity to apply practical applications covering a variety of tasks such as computer vision, natural language processing, product recommendation and more. Leaving this workshop, you should have a firm grasp of deep learning and be able to implement a systematic approach for producing high quality modeling results.

## Is this course for me?

Is this workshop for you? If you answer "yes" to these three questions, then this workshop is likely a good fit: 

1. Are you relatively new to the field of deep learning and neural networks but eager to learn? Or maybe you have applied a basic feedforward neural network but aren’t familiar with the other deep learning frameworks? 

2. Are you an experienced R user comfortable with the tidyverse, creating functions, and applying control (i.e. if, ifelse) and iteration (i.e. for, while) statements? 

3. Are you familiar with the machine learning process such as data splitting, feature engineering, resampling procedures (i.e. k-fold cross validation), hyperparameter tuning, and model validation? 

This workshop will provide some review of these topics but coming in with some exposure will help you stay focused on the deep learning details rather than the general modeling procedure details.

## Prework

I make a few assumptions of your established knowledge regarding your programming skills and machine learning familiarity (items #2-3 in the previous section). Below are my assumptions and some resources to read through to make sure you are properly prepared.

| Assumptions                       | Resource      
| --------------------------------- | ------------- |
| You should be familiar with the Tidyverse, control flow, and writing functions | [R for Data Science](https://r4ds.had.co.nz/) | 
| You should be familiar with the basic concept of machine learning | [Ch. 1 HOMLR](https://bradleyboehmke.github.io/HOML/intro.html) | 
| You should be familiar with the machine learning modeling process | [Ch. 2 HOMLR](https://bradleyboehmke.github.io/HOML/process.html) | 
| You should be familiar with the feature engineering process | [Ch. 3 HOMLR](https://bradleyboehmke.github.io/HOML/engineering.html) |


You will require several packages and datasets throughout this workshop. If you are attending the workshop these will be preinstalled for you so you do not need to worry about your OS differing from mine. However, after you leave the workshop, the first notebook below will allow you to reproduce the work you did in the workshop. Also, at the conference workshop, we will all use the RStudio Cloud platform. The second notebook below will get you set up so that we can hit the ground running on day 1!

| Description                       | Resource
| --------------------------------- | :-------------: |
| Pre-installing necessary packages and datasets (already pre-installed for workshop!) | [Instructions](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/01-intro/01-requirements.md) <br> [Source Code](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/01-intro/01-requirements.Rmd) |
| Setting up RStudio Cloud environment | [Instructions](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/01-intro/02-server-instructions.md) |

## Schedule

This workshop is notebook-focused. Consequently, most of our time will be spent
in R notebooks; however, I will also jump to slides to explain certain concepts
in further detail. Throughout the notebooks, you will see ℹ️ icons that will
hyperlink to relevant slides (or additional resources).

### Day 1

| Time          | Activity                             | Notebook      | Source Code   | Other    |
| :------------ | :----------------------------------- | :-----------: | :-----------: | :------: |
| 09:00 - 09:30 | Introduction                  |          |             | [Slides](https://rstudio-conf-2020.github.io/dl-keras-tf/01-intro.html#1) |
| 09:30 - 10:30 | Deep learning ingredients  | [Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/01-main-ingredients.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/02-main-ingredients/01-main-ingredients.Rmd) | [Slides](http://bit.ly/dl-01) |
| 10:30 - 11:00 | *Coffee break*                |   |   |   |
| 11:00 - 12:30 | Deep learning recipe |   |   |   | 
|               | &nbsp;&nbsp;&nbsp;Training your model |[Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/01-starter-recipe.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/03-recipe/01-starter-recipe.Rmd) |   |
|               | &nbsp;&nbsp;&nbsp;Mini-project: Predicting Ames, IA home sales prices | [Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/02-mini-project-ames.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/03-recipe/02-mini-project-ames.Rmd) | [Solution](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/ames-mini-project-solution.nb.html)  |
| 12:30 - 13:30 | *Lunch break*                 |   |   |   |
| 13:30 - 15:00 | Computer vision & CNNs        |   |   |   |
|               | &nbsp;&nbsp;&nbsp;MNIST revisted | [Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/01-mnist-revisited.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/04-computer-vision-CNNs/01-mnist-revisited.Rmd) | [Slides](http://bit.ly/dl-03#12) |
|               | &nbsp;&nbsp;&nbsp;Cats vs dogs | [Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/02-cats-vs-dogs.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/04-computer-vision-CNNs/02-cats-vs-dogs.Rmd) | [Slides](http://bit.ly/dl-03#37) |
|               | &nbsp;&nbsp;&nbsp;Transfer learning | [Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/03-transfer-learning.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/04-computer-vision-CNNs/03-transfer-learning.Rmd) | [Slides](http://bit.ly/dl-03#45) |
| 15:00 - 15:30 | *Coffee break*                |   |   |   |
| 15:30 - 17:00 | Project: Classifying natural images  | [Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/01-Project.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/05-project/01-Project.Rmd) | [Solution](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/project1-natural-images.nb.html) |

### Day 2

| Time          | Activity                             | Notebook      | Source Code   | Other    |
| :------------ | :----------------------------------- | :-----------: | :-----------: | :------: |
| 09:00 - 10:30 | Word embeddings               |   |   |   |
|               | &nbsp;&nbsp;&nbsp;The original IMDB | [Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/01-word-embeddings.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/06-word-embeddings/01-word-embeddings.Rmd) | [Slides](http://bit.ly/dl-06) |
|               | &nbsp;&nbsp;&nbsp;Pre-trained embeddings | [Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/02-pretrained-word-embeddings.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/06-word-embeddings/02-pretrained-word-embeddings.Rmd) | [Slides](http://bit.ly/dl-06) |
|               | &nbsp;&nbsp;&nbsp;Mini project - Amazon reviews | [Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/03-your-turn-amazon-word-embeddings.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/06-word-embeddings/03-your-turn-amazon-word-embeddings.Rmd) | [Solution](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/project-embeddings-amazon-reviews.nb.html) |
| 10:30 - 11:00 | *Coffee break*                |   |   |   |
| 11:00 - 12:30 | Collaborative filtering       | [Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/collaborative-filtering.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/07-recommender-collaborative-filtering/collaborative-filtering.Rmd) | [Excel file](http://bit.ly/dl-07-Excel) |
| 12:30 - 13:30 | *Lunch break*                 |   |   |   |
| 13:30 - 15:00 | RNNs & LSTMs             |   |   |   |
|               | &nbsp;&nbsp;&nbsp;IMDB revisted | [Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/01-intro-to-lstms.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/08-NLP-LSTMs/01-intro-to-lstms.Rmd) | [Slides](http://bit.ly/dl-08) |
|               | &nbsp;&nbsp;&nbsp;Mini project - Non-IMDB reviews | [Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/02-your-turn-lstms.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/08-NLP-LSTMs/02-your-turn-lstms.Rmd) | [Solution](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/02-your-turn-lstms-solution.nb.html) |
| 15:00 - 15:30 | *Coffee break*                |   |   |   |
| 15:30 - 17:00 | Wrap up                       |   |   |   |
|               | &nbsp;&nbsp;&nbsp;Project: Detecting Duplicate Quora Questions | [Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/Final-Project.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/09-project/Final-Project.Rmd) | [Solution](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/02-Project-solution.nb.html) |
|               | &nbsp;&nbsp;&nbsp;Final words of wisdom |   |   | [Slides](https://rstudio-conf-2020.github.io/dl-keras-tf/09-wrap-up.html) |

### Extras

| Activity                      | Notebook | Source Code |
| :---------------------------- | :--------: | :-----------: |
| Improving generalization with k-fold cross validation       | [Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/validation-procedures.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/99-extras/validation-procedures.Rmd) |
| Performing a grid search | [Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/imdb-grid-search.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/99-extras/imdb-grid-search.Rmd) |
| Linear regression with stochastic gradient descent | [Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/manual-gradient-descent.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/99-extras/manual-gradient-descent.Rmd) |
| Diagnosing model performance with learning curves | [Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/learning-curve-diagnostics.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/99-extras/learning-curve-diagnostics.Rmd) |
| Save your models for later with serialization | [Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/save-your-models.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/99-extras/save-your-models.Rmd) |
| Visualizing what CNNs learn | [Notebook](https://rstudio-conf-2020.github.io/dl-keras-tf/notebooks/visualizing-what-cnns-learn.nb.html) | [.Rmd](https://github.com/rstudio-conf-2020/dl-keras-tf/blob/master/materials/99-extras/visualizing-what-cnns-learn.Rmd) |


## Instructor

<img src="https://avatars2.githubusercontent.com/u/6753598?s=460&v=4" width="100"/>

Brad Boehmke is a Director of Data science at 84.51° where he wears both
software developer and machine learning engineer hats. His team focuses
on developing algorithmic processes, solutions, and tools that enable
84.51° and its data scientists to efficiently extract insights from data
and provide solution alternatives to decision-makers. He is a visiting
professor at the University of Cincinnati, author of the _[Hands-on
Machine Learning with R](https://www.crcpress.com/Hands-On-Machine-Learning-with-R/Boehmke-Greenwell/p/book/9781138495685)_ and [_Data Wrangling with R_](https://www.springer.com/us/book/9783319455983)
books, creator of multiple public and private enterprise R packages, and developer of
various data science educational content. You can learn more about his
work, and connect with him, at [bradleyboehmke.github.io](http://bradleyboehmke.github.io/).

## TAs

<img src="https://avatars2.githubusercontent.com/u/4276246?s=400&v=4" width="100"/>

__Rick Scavetta__

<img src="https://assets.datacamp.com/users/avatars/000/254/434/medium/B7H1-OMAYMA_SAID.jpg?1534974674" width="100"/>

__Omayma Said__

<img src="https://avatars3.githubusercontent.com/u/5878305?s=460&v=4" width="100"/>

__Doug Ashton__

<img src="https://avatars3.githubusercontent.com/u/1580714?s=460&v=4" width="100"/>

__Daniel Rodriguez__

-----

![](https://i.creativecommons.org/l/by/4.0/88x31.png) This work is
licensed under a [Creative Commons Attribution 4.0 International
License](https://creativecommons.org/licenses/by/4.0/).
