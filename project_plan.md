# Project Plan
## Discourse Analysis 
#### Summary
Unlike a natural conversation, discourse within online forums occurs asynchronously and (largely) anonymously. This project will be an analysis of how conversations within individual Reddit posts develop. The data will then be compared to other posts within the same subreddit, then all subreddits will be compared to one another.
#### Data
Data will be pulled from reddit using the Reddit API and will cover a variety of subreddits. [r/AskReddit](https://www.reddit.com/r/AskReddit/) will be used, since the subreddit is conversational in nature, as well as [r/politics](https://www.reddit.com/r/politics/) and other to-be-determined subreddits. Data cleaning and scraping will not be a huge hurdle due to the existing [Reddit API](https://www.reddit.com/dev/api/). If time permits, discourse analysis will be performed on natural conversation data to serve as a point of comparison.
#### Analysis
In exploring this data, I would look for differences in how conversations develop within individual reddit posts, and whether popoular posts in a subreddit lead to the appearance of other related posts. In this analysis, I will explore the concept of turn-taking in online discourse, as well as look at the different ways users respond to . Do complex, highly-detailed posts result in equally as complex responses? [Another question to ask is, do different speech acts (threatening, questioning, etc.) result in different types of responses?](https://www.researchgate.net/publication/317179480_Analyzing_Online_Discourse_Some_Theoretical_Ideas_and_a_Visualization_Approach_Research-in-Progress) (Beaulieu, Tanya & Sarker, Suprateek & Sarker, Saonee 2015). Do speech acts of the same classification tend to fall on the same end of the sentiment spectrum? These questions will be probed for each subreddit, then compared side-by-side to see if discourse around certain topics carry their own patterns, or if there is a universal structure of discourse on Reddit.
#### Presentation
Graphs and statistical tests will be performed within Jupyter Notebooks, which will then be compiled into a final report and contextualized/explained.

Referenced Papers:
Beaulieu, Tanya & Sarker, Suprateek & Sarker, Saonee. (2015). Analyzing Online Discourse: Some Theoretical Ideas and a Visualization Approach Research-in-Progress. 