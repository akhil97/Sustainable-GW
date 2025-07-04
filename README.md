# Sustainable-GW

## The official repository for information on GW DSSD's research project on the Yellowknife, Canada wildfire evacuation.

Yellowstone Wildfire Social Media Analysis

This project analyzes social media posts from a Facebook group to understand the key topics of conversation during the Yellowstone wildfire. By using natural language processing (NLP) and topic modeling, we can get a clearer picture of the community's concerns, information sharing, and support systems during this critical event.

Project Scope

The goal of this project is to sift through a large number of social media posts and automatically identify the main themes or topics that people were discussing. This can help us understand:

    What were the most pressing concerns for people affected by the wildfire?

    How was information about safety, evacuation, and resources being shared?

    What were the common messages of support and community assistance?

By understanding these conversations, we can learn valuable lessons for future emergency response and community support efforts.

About the Dataset

The data for this project comes from a scrape of a Facebook group, saved in the apify_group_scrape.csv file. The dataset includes the following information for each post:

    Poster: The name of the person who made the post.

    Content: The text of the post itself.

    Comments: The number of comments on the post.

    Reactions: The number of reactions (likes, hearts, etc.) to the post.

    Reposts: The number of times the post was shared.

    Time: The date and time the post was made.

In total, there are 405 posts in the dataset.

Word Cloud Analysis

A word cloud is a visual representation of the most frequently used words in a collection of text. The larger the word, the more often it appeared in the social media posts. This gives us a quick, at-a-glance view of what was on people's minds.

Here's the word cloud generated from the social media posts:

As you can see, words like "safe," "Edmonton," "river," "high," and "level" are prominent, which immediately tells us that safety and specific locations were major topics of conversation.

Key Findings

We used a technique called Latent Dirichlet Allocation (LDA) to automatically group the posts into different topics. We identified 5 main topics of conversation:

    Topic 1: Checking In and Safety Status: This topic is dominated by words like "anyone," "safe," and "Edmonton." This suggests that a major part of the conversation was people checking on each other's safety and sharing their location, particularly in relation to Edmonton.

    Topic 2: Evacuation and Support Centers: With words like "Edmonton," "safe," and "centre," this topic likely revolves around discussions about evacuation centers and the support being offered in Edmonton.

    Topic 3: Peace River and Safety: This topic highlights "river," "peace," and "safe," indicating that the Peace River area was another significant location for safety check-ins and discussions.

    Topic 4: High Level and Safety: The words "high," "level," and "safe" point to conversations centered around the High Level area and the safety of people there.

    Topic 5: General Information and Evacuee Status: This topic, with words like "fyi," "fort," and "evacuee," seems to be about sharing general information and updates for evacuees.

How to Use This Project

To run this analysis yourself, you will need to have Python and Jupyter Notebook installed. You'll also need to install the following libraries:

pip install pyLDAvis
pip install nltk
pip install pandas
pip install scikit-learn
pip install wordcloud
pip install matplotlib
pip install gensim
pip install spacy

Once you have these installed, you can run the Yellowstone_wildfire_topic_modelling_gensim_LDA.ipynb notebook to see the analysis step-by-step. You will also need the apify_group_scrape.csv file in the /content/sample_data/ directory for the notebook to run correctly.

