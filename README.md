## Uber pick-ups project
Uber's data team would like to work on a project where the app would recommend hot zones in major cities to be in at any given time of day.

## Goal
- Devise a method to determine where are the hot zones per hour per day
- Use two unsupervised learning algorithm (DBSCAN and K-means) for this project
- Show hot zones on an interactive dashboard where the user could just press the play button and see the evolution for each hour

## Methodology
- The first intuition while reading this project was to use DBSCAN. Given that the number of clusters had not to be specified, the DBSCAN algorithm has been used right away to solve the problem. Different epsilon and min_sample values have been used to obtain the most appropriate results. However, I must admit that I am not satisfied with the different clusters I have obtained.
- K-means clustering algorithm was also used to solve the Uber pick-ups problem. The Elbow and Silhouette methods have been applied to find the optimal number of clusters.

## Constraints
- Processing the huge dataset required much time. To reduce processing time, a random sample of 100 000 observations was taken from the original dataset.
- Another drawback was my poor knowledge of New York City. I tried to gain some domain knowledge by web searches but it was quite frustrating not being able to know whether the clustering algorithm was performing well or not.

## Conclusion
- The overall result with DBSCAN was not satisfying. I will work on this project again and try to test how other hyperparameters (Euclidean distance instead of Manhattan distance, for example) influence the DBSCAN algorithm.
