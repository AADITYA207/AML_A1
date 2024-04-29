We have prepared the recommender system using a pre-trained sentence transfomers called "all-mpnet-base-v2".
We first extracted the summary of each paper from the paper_of_interest csv file. 
Then, using this sentence transformer we generated contextual embeddings of the abstract of papers from the daily_arxiv.csv and the summary of paper_of_interest.csv
Then, we have used cosine similarity and euclidean distance for each paper in paper_of_interest, to find the papers with the max cosine similarity and least euclidean distance, and suggested them as similar to our query papers.