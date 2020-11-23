# IMDB-Movie-Reviews-50k

This Repository includes the data set from [1], described in [2], reorganised  into plain excel files. They can be  loaded more easily and applied to different tasks straightforwardly. The tables include all provided information, as review text, rating (0 to 10) and Sentiment (pos, neg). 

 

### Structure

The frames include six columns each.  **ID** are unmodified IDs from the original data set [1]. They are individual within each subset and in the range of 0 - 12499. (Subsets are training positive, training negative, test positive and test negative.)
While the **Review** column includes the original Markdown review texts, **Review clean** provides a preprocessed version of that. In the preprocessing, all letters were lowered and punctuation and irregular symbols have been removed.  
The **Rating** is the IMDb rating from 1 to 10 that is associated to that review. Note that the dataset does not contain reviews with rating 5 or 6. Reviews are grouped in positive (7-10) and negative (1-4) sentiments, which is indicated by **Sentiment**. The column **Set** specifies whether this rating is part of the training or test set.

The attached notebook (*load_data.ipynb*) gives a basic instruction for loading the data, along with some basic examples how to split the data for different purposes.



---
### Reference
[1] https://ai.stanford.edu/~amaas/data/sentiment/   
[2] Maas, A., Daly, R. E., Pham, P. T., Huang, D., Ng, A. Y., & Potts, C. (2011, June). Learning  word vectors for sentiment analysis. In Proceedings of the 49th annual meeting of the association for computational linguistics: Human language technologies (pp. 142-150).