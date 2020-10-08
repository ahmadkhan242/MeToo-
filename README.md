# MeToo-
IEEE BigMM Grand Challenge  
This grand challenge involves creating multi-task multimodality frameworks aiming at predicting labels for a given tweet.
***
## Dataset 
> Availabe on [Kaggel](https://www.kaggle.com/c/ieee-bigmm-data-challenge)  
The dataset contains 9,973 tweets manually annotated into the aforementioned linguistic aspects. The labels are:  
* Relevance: This category utilizes image and text labels aimed to identify if the tweet is related to the MeToo movement. Relevant tweets include personal opinions, instances of abuse, support for the victims of the campaign, or links to the news articles.  
* Stance: Stance detection label helps to understand the public opinion about a topic and also has downstream application tasks. Stance detection labels are segregated into three categories: Support, Opposition, Neither. Support includes tweets that expressed appreciation of the MeToo movement, shared resources for victims of sexual abuse, or offered empathy towards the victims.  
* Hate Speech: Detection of hate speech has been gaining interest in linguistic research lately. For a given tweet, the hate speech was distributed into Directed Hate and Generalized Hate.  
* Sarcasm: Sarcasm detection is of interest in areas like sentiment analysis and affective computing. The tweet has been marked as sarcastic if it includes details about an individual involved, an entity, or the movement in humorous overtone.  
* Dialogue Acts: A dialogue act is defined as a function of the speaker's utterance during the conversation. The dataset includes dialogue acts that are specific to the MeToo movement: Allegation, Refutation, and Justification.  
## Models Used
###  Convolutional Neural Nets  
    Layers: 3  
    Kernels: 5, 7, 8  having 512 filters each  
    Final layer: Dense, 10 units, Sigmoid activation  
### Bidirectional LSTMs  
    Layers: 2, bi-bidirectional
    Units: 128
    Final layer: Dense, 10 units, Sigmoid activation
### Pre-trained BERT
    Model: BERT Large un-cased Pre-trained
### An Ensemble of the above three models.


