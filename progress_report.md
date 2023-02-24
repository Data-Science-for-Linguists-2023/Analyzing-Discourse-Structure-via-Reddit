# Progress Reports

## Preliminary Report
Set up project repository and cleaned up project plan. Placeholder for the License has been created, as well as a readme. 
## 1st Progress Report
This report focuses primarily on data collection and exploration, which can be found within data_collection.ipynb. This data includes 'hot (trending)' posts from the [politics](https://www.reddit.com/r/politics/), [AskReddit](https://www.reddit.com/r/AskReddit/), [soccer](https://www.reddit.com/r/soccer/), [happy](https://www.reddit.com/r/soccer/), and [music](https://www.reddit.com/r/music/) subreddits. These were chosen due to the likelihood of their topics sparking conversation. 

Prior to writing this progress report, the following was accomplished:
* A [RedditAPI](https://www.reddit.com/dev/api/) application was setup to allow for data to be pulled from Reddit
* [PRAW](https://praw.readthedocs.io/en/stable/) was installed as a tool for interacting with the RedditAPI
* Data from each subreddit's 20 rising posts were extracted and placed into dataframes with their comment structure in-tact
* The comment structure of posts was explored. Comments are stored in CommentForest objects, which contains every comment and reply to a post. When using the list() function, comments are displayed using BFS
* The list() function was found within [PRAW's open-source GitHub repository](https://github.com/praw-dev/praw/), and the process of modifying it for DFS has begun

#### Sharing Plan

For the sharing plan, I plan on finding a way to quantify different aspects of discourse and their frequency within each post. I will use DFS to display comment chains from within the posts I am using, which will be displayed in DFS fashion. Regarding the CSV files, a better way must be found to store comments. This will be explored when DFS is fully functional for CommentForest objects. 