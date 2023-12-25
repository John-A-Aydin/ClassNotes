### Netflix data set 
[Link](https://www.kaggle.com/datasets/maso0dahmed/netflix-movies-and-shows/data)
## Ideas

### Title length

1. Find out if there is any correlation between title length, in both characters and words, and number of imdb ratings.
2. Find out if the number of imdb ratings is correlated with the actual rating of the show

|                 | **High # of IMDB ratings**                          | **Low # of IMDB ratings**       |
| -------------------- | --------------------------------------------------- | ------------------------------- |
| **High star rating** | Show likely got views on its merits                 | Show didn't reach enough people |
| **Low star rating**  | Show reached a lot of people, but not on its merits | Bad show                        |

If we find that shows within a certain title length fall into a low number of ratings with a high star rating it could mean that the title length was unoptimal

If we find that shows within a certain title length fall into a high number of ratings with a low star rating it could mean that the title length is optimal to get people to watch

### Runtime

Same as title length just with runtime 
Honestly think this is a better idea.
Could also look at how it changes over time. 
- Does the popularity vs runtime change over time?
- Wouldn't actually apply bc the imdb ratings are too recent (not made on release of show)

### Important

Look for data points that have a high correlation with high number of imdb ratings, but low star rating 

#### Multiple predictors

Check lect 8 slides and create that matrix with data set
See hyper plane

$\large\text{runtime, title lenght, } \rightarrow \text{number of imdb ratings}$