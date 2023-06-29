# final-project
## “What words are most characteristic for the the Guardian top 100 novels?”.
Additionally: “Can you use summaries of books to find characteristic words?”

To answer the research question, I used beautiful soup to scrap the top 100 books from the Guardian. Then I scrap genres, authors, and
descriptions from the Goodreads website using iterations to make sure I get everything I want. 
Furthermore, I tokenize the description using spaCy which is a pre-trained model. I choose the appropriate token and only use the lemma for top 1000 frequency. 
I then used Gensim to create a dictionary for tokens and used an LDA modelling (C_v algorithm) to come up with 6 topics for PCA which has 
the relatively highest coherence score and set my topics to 5. By training an LDA model I visualize the topics' distribution and the most relevant terms for 
each topic. In the end, I find intresting topics by comparing the topics by PCA and comparing them to the genres.
