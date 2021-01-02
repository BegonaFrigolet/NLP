# Natural Language Processing 

# Analyzing Domestic Violence through Topic Modelling

Domestic Violence is not a pandemic, it’s an epidemic. With Covid-19 ravaging the economy; increasing unemployment such crises are set to become much more frequent. Add another public health crisis to the toll of the new coronavirus: Mounting data suggests that domestic abuse is acting as an opportunistic infection, flourishing in the conditions created by the pandemic.

As this problem has serious precautions on the physical and mental health of the victims (children, woman, man), a lot of research has been already conducted to analyse the nature of this social problem from interviews with victims, and official data like health records. Recently there has been significant effort put into social media data research. However, much of this research found has many limitations to create practical tools to deal with domestic violence. Within this project, we are looking utilizing topic modelling to assist with domestic violence data classification.

# Final Report: 
- Final Report can be found in this link
- Final Presentation can be found in this link
- Final Website & Application can be found in this link

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

This Project was done in collaboration with Marang Mutloatse Adelina Akhsanova, Nisrine Ferahi, Begona Frigolet, Mohamed Amer and Prasanth Chakka.
