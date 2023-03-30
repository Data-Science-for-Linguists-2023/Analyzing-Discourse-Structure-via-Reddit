# Progress Reports

## Preliminary Report
Set up project repository and cleaned up project plan. Placeholder for the License has been created, as well as a readme. 
## 1st Progress Report
This report focuses primarily on data collection and exploration, which can be found within data_collection.ipynb. This data includes 'hot (trending)' posts from the [politics](https://www.reddit.com/r/politics/), [AskReddit](https://www.reddit.com/r/AskReddit/), [soccer](https://www.reddit.com/r/soccer/), [happy](https://www.reddit.com/r/happy/), and [music](https://www.reddit.com/r/music/) subreddits. These were chosen due to the likelihood of their topics sparking conversation. 

Prior to writing this progress report, the following was accomplished:
* A [RedditAPI](https://www.reddit.com/dev/api/) application was setup to allow for data to be pulled from Reddit
* [PRAW](https://praw.readthedocs.io/en/stable/) was installed as a tool for interacting with the RedditAPI
* Data from each subreddit's 20 rising posts were extracted and placed into dataframes with their comment structure in-tact
* The comment structure of posts was explored. Comments are stored in CommentForest objects, which contains every comment and reply to a post. When using the list() function, comments are displayed using BFS
* The list() function was found within [PRAW's open-source GitHub repository](https://github.com/praw-dev/praw/), and the process of modifying it for DFS has begun

## 2nd Progress Report
This report focuses on the following goals (bolded means the task has been completed):
* **Completing data acquisition**
* **Cleaning and reorganizing data**
* **Finalizing the sharing scheme**
* **Finalizing licensing**
* Starting analysis

#### Data Acquisition

New data, and more of it, was acquired. 100+ posts from 5 different subreddits (same as before, but r/happy was replaced by [UpliftingNews](https://www.reddit.com/r/UpliftingNews/)) were pulled, all with their own pools of comments.

#### Cleaning and Reorganizing

The data has been narrowed down into the relevant columns for this analysis, and for readability's sake, I have modified the list() function provided by PRAW into a depth-first search vs. a breadth-first. A breadth-first search means it first displays first-level comments (directly to the post), then second-level comments (responses to first-level comments), etc., with no particular order to them. Displaying them depth-first gives conversation chains first and foremost.

#### Sharing Scheme

Information is available at the bottom of this document

#### Licensing

I chose the GNU General Public License 3.0, as it will allow for my data and results to be used, modified, and distributed freely. The license can be found [here](https://github.com/Data-Science-for-Linguists-2023/Analyzing-Discourse-Structure-via-Reddit/blob/main/LICENSE)

#### Analysis

The approach I want to take for analysis is still being considered. There is a limitation to analyzing long conversation chains, which is that comments beyond a certain level are stored as 'MoreComments' objects instead of objects, which do not contain text data. Lower-level comments are typically the richest in data, but this is still a loss of information. The approach of considering each comment in isolation is being considered, and seeing if certain components/characteristics result in more responses.

#### Sharing Plan

For the sharing plan, I have pickled all of my dataframes, which are available [here](https://github.com/Data-Science-for-Linguists-2023/Analyzing-Discourse-Structure-via-Reddit/tree/main/datasamples)

As [Reddit's API Terms of Use](https://github.com/Data-Science-for-Linguists-2023/Analyzing-Discourse-Structure-via-Reddit/tree/main/datasamples) state, I am free to display and freely distribute my data (though, if told to by Reddit, I will take it down). 