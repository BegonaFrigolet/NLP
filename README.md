# Natural Language Processing 

# Analyzing Domestic Violence through Topic Modelling - All documentation can be found on this [LINK](https://github.com/BegonaFrigolet/Natural-Language-Processing/tree/main/NLPAssignment_GroupA).

Domestic Violence is not a pandemic, it’s an epidemic. With Covid-19 ravaging the economy; increasing unemployment such crises are set to become much more frequent. Add another public health crisis to the toll of the new coronavirus: Mounting data suggests that domestic abuse is acting as an opportunistic infection, flourishing in the conditions created by the pandemic.

As this problem has serious precautions on the physical and mental health of the victims (children, woman, man), a lot of research has been already conducted to analyse the nature of this social problem from interviews with victims, and official data like health records. Recently there has been significant effort put into social media data research. However, much of this research found has many limitations to create practical tools to deal with domestic violence. Within this project, we are looking utilizing topic modelling to assist with domestic violence data classification.

## Final Report & Applications: 
- To Review  the Website & Application can be found in this [LINK](https://bfdelavega.wixsite.com/misitio)
- To Review  the Final Report can be found in this [LINK](https://github.com/BegonaFrigolet/Natural-Language-Processing/blob/main/NLPAssignment_GroupA/Final%20Report_GroupA.pdf)
- To Review  the Final Presentation can be found in this [LINK](https://github.com/BegonaFrigolet/Natural-Language-Processing/blob/main/NLPAssignment_GroupA/GroupA_Domestic_Violence.pptx)

## Data & Methodology: 

### Methodology: 
- Topic modelling is a text mining technique which provides methods for identifying co-occurring keywords to summarize large collections of textual information. It helps in discovering hidden topics in the document, annotate the documents with these topics, and organize a large amount of unstructured data.

- Techniques Applied: Latent Dirichlet Allocation (LDA), Hierarchical Dirichlet Process (HDP)

### Data: Data is scraped online on twitter, reddit and from online news articles. Specific hashtags Hashtags used for every file for twitter:
- 1 = METOO
- 2 = WHYISTAYED WHYILEFT
- 3 = HeForSheAtHome WomenCount GenerationEquality, AntiDomesticViolenceDuringEpidemic Mask-19 WithHer SpotlightEndViolence
- 4 = staysafe domesticviolence DomesticAbuse DomesticViolence

## Our Purpose:
- The online content generation has grown rapidly in scale. The unstructured and noisy character of such data has further added to an overall complexity of processing and utilizing available information. The mix of messages that are of personal nature in a form of mere opinions or empathetic thoughts along with general awareness promotions have greatly diminished the DVCS services efficacy.
- With topic modelling, we are looking to identify the different topics or classes of the tweets or comments in reddit platform to make the large and unstructured data more organized in a way that will make it easier for NGOs, government officials or researchers to assess and get useful insights from to better analyze this crisis and come up with better courses of actions accordingly.
- At present, there is no available benchmark dataset for domestic violence with pre-labeled data for multiclass classification, so it is a very manual intensive job. Topic modelling could help identify the different topics so it is easier to build a corpus later with labeled data that can serve as a training dataset for deep learning algorithms like CNNs and RNNs for classifying domestic violence texts.


## Findings: 

### Reddit
- Through all the comments, mainly women are seeking help, sharing their abuse stories, how they survived and how they want to help other people.
- One of the main insights is that the most important topic is about family abuse, not relationship abuse, mentioning mother, father, relationship and child as well as kid, we assume that these people are young adults or teenagers living with their families.
- Time is also a concept that is frequent among all topics, quoting "year", "month", "day" as important words describing the testimonies.
#### Recommendations Reditt
- Organizations and NGO should have initiatives and communication through Reddit since it is a space in which people share their testimonies, is a channel where the initiatives can be communicated to the right people.
- Partner abuse is highly related to partner abuse.

### Twitter: All Data
- Through all the tweets the main conversation is from organizations and movements to invite people to join the movements through hashtags and facts, we can also perceive not only organizations but sponsors.
- Below are the relevant inferred topics:
- Topic 1: #WHYILEFT, #METOO, #WITHHER - This movement revolves around raising awareness and acting with the organization - ipu parliament (global organization of national parliaments to promote peace, democracy and sustainability), also the sponsorship of women in sport.
- Topic 2: #METOO, #believewoman - Victims sharing their stories and support of one another and sharing their survivor stories, organization - ipu parliament (global organization of national parliaments to promote peace, democracy and sustainability), also the sponsorship of women in sport.
- Topic 3: #genderequality - Feminism and equality - Backed by the organization "everyday equality" to drive equal social opportunities in UK.
- Topic 4: timesup - Campaign to report and end violence thus creating an equal future, promoting also job quality and activism.
- Topic 5: Abuse regarding rape in family and work – organization like Orange the World: Generation Equality Stands against Rape.
- Topic 6: Promotes discussion of psychological abuse, harassment and solution making.

#### Our final insights
On Twitter is about joining the conversation and promoting the initiatives and campaigns, identified movements:#whyistayed, #metoo,#timesup,#heforshe,#iwillgoout,#yesallwomen,#orangetheworld,#niunamenos ,#everydaysexism,#womenshould

- Recommendations
An improvement that can be done in twitter is not only promote de initiatives and join the conversation but invite victims to share their story via Reddit, because there is no character limit, thus increasing Reddit ́s testimonies and having more information regarding this subject.

This Project was done in collaboration with Marang Mutloatse Adelina Akhsanova, Nisrine Ferahi,Mohamed Amer and Prasanth Chakka.



# Analyzing Disaster Tweets Through NLP All documentation can be found on this [LINK](https://github.com/BegonaFrigolet/Natural-Language-Processing/tree/main/NLP%20%20Disaster%20Tweets).


### Main Goal: 
The goal is to try to help the prediction of which Tweets are talking about real disasters and which ones are not. The problem is dealing with a binary classification problem classifying them The data set is of 10K tweets that were hand classified, from the company figure-eight and originally shared on their "Data For Everyone" website here.

Tweet source: https://twitter.com/AnyOtherAnnaK/status/629195955506708480

### Techniques:
Due to counter vector giving longer documents I used TF- IDF, which does not only represent if the words are there or not, instead represent the frequency and their inverse document frequency, thus giving less significance to the words that are frequent but appear everywhere, and gives higher value to the words that appears frequently but only in few places.

Other  Techniques Applied: 
- Stop Words
- Removing Punctuation/URL/HTML
- Lemmatization
- Stemming
#### Classifiers: 
- SVM + Lemmatization
- Log Regression + Lemmatization

### Process:
The process of predicting whether or not the tweets are about real disaster tweets, was getting to know the data, thus doing the Exploratory Analysis, making the first important observation:

There are three columns with relevant information: "Location","Keyword" and "Text". For training the model the column "text" will be the main one since I have to convert the text files into numerical features.

The distribution of words are not different on classification, and the data is not imbalanced.

Building a baseline:

For building the baseline, I used Count Vectorizer in order to run the model, I need to convert the text files into numerical features.

Count Vectorizer, similar to One-Hot encoding, segments the text feature into words, which are split by "space" and count the number of times the word appears, finally it assign an ID.

Due to counter vector giving longer documents I used TF- IDF, which does not only represent if the words are there or not, instead represent the frequency and their inverse document frequency, thus giving less significance to the words that are frequent but appear everywhere, and gives higher value to the words that appears frequently but only in few places.

Afterwards I used Naive Bayes Multinomial as the model,goal is that the probability of the classification being 0 is bigger than 1.

Also I used a pipeline, the reason for Naive Bayes is that it has that theorem built in and for the pipeline feature because it allows an end to end processing, implementing count vectorizer, TF-IDF and the model, as well as not needing to do it on test as well.

Baseline Score: 0.79652 in Kaggle.

After the Baseline I started with pre-processing and cleaning the data.

Starting with Stop words in English and N-grams from 1 to 3, having from N-gram to trigram, which I included in Count Vectorizer resulting on: 0.79345.

For cleaning the data, I analyzed which words were the most used and stummble upon the conclusion that they were:HTTP HTML thus decided to remove them as well as the punctuation which included hashtags and mentions (#,@)

Text Normalization:

I tried both Lemmatization and Stemming:

Lemmatization: Is the process that uses a corpus to return the from of a word.
Stemming- Removing the first and last section of the word, which for english language works.
The difference between both was slightly better on "Lemmatization"

After Text normalization, I tried different classification Models:

1.SVM: Which is an improvement of Multinomial, and is more effective in high dimensions and Spaces.

Trying Logistic Regression.
Both of them with Lemmatizing and Stemming:

Both had a good performance, being SVM the best one, and after applying the best of all of them: Lemmatization, fixing punctuation, stop stop words and SVM, I got my best score: 0.80368 out all of the tried things.

After getting that score I tried to ran other word embedding, which I could not make work but I thought they were very interesting I tried:

Word2Vec: is a very powerful tool, because instead of counting how often a word occur with another it predicts how likely a word is going to show given another one.
For me it did not ran properly taking a lot of time, thus not having a proper conclusion, I will keep trying it to run it further on, but for this project it did not work.

Glove: After doing the model the score is .778, thus not improving, I tried it and think I have to read more about it and optimize, but I do not think this is quite correct. But I think is a very good embedding in theory, since it takes a global occurrence of words with other words, with the before and after and what is the frequency, thus being a very powerful embedding.
After doing this project I have learned a lot about NLP and how to optimize the predictions tweets, one of my biggest learnings was not repeating the same process, which I did removing punctuations due to me using the pipeline.

### Main Insights:

 - Distributions of words for my case were not as relevant as removing the stop words all together, due to the distribution being similar on both classes.

-  The pre processing methologies that worked the most was "Lemmatization"& "Removal of stopwords, html, punctuation and Url". Stemming decreased the score on its own and when mixing them with other classifiers was lower than Lemmatization.

-  Ngrams optimization from 1 to 3 was worth it as it optimizes within the possible combinations looking for one up to 3 words, which increased the performance better than not placing it.

-  TTF-IDF: This implementation was absolutely worthy and necessary, because of the description that I made earlier by assigning a weight to the words, and the performance did increase specially when blended with lemmatization and text clean up.



