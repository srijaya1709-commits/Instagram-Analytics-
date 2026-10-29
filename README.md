# Instagram Analytics

Exploratory data analysis (EDA) of an Instagram posts dataset (about 30,000 posts) to understand what drives engagement.

**Author:** Jaya Sri C
**GitHub:** [srijaya1709-commits](https://github.com/srijaya1709-commits)

## What this project does
- Loads the dataset and checks for missing values
- Calculates mean, median, mode and standard deviation for key metrics: follower count, likes, comments, shares, saves, reach, impressions and engagement rate
- Visualizes the data:
  - Line chart: monthly average followers gained
  - Horizontal bar chart: total posts per content category
  - Scatter plot: reach vs. likes, colored by media type (Reel, Image, Carousel)
  - Scatter plot with a regression trendline
- Uses `groupby()` to compare average likes and reach across content categories

## Key insights
1. The dataset has about 30,000 posts with no missing values. A typical post reaches about 4,900 people and gets about 199 likes (median). The mean is 288 because a few viral posts pull it up.
2. Reach is the strongest driver of likes (r = 0.74), but the link is loose. Many posts with 20,000+ reach still got under 1,000 likes, so content quality matters as much as visibility.
3. Engagement rate stays near 4% and followers gained stays near 500 per post across the year (488 to 510), so there is no clear growth or seasonal trend.
4. Content categories are evenly split at about 3,000 posts each, and image, carousel and reel perform in a similar range, so no category or format is a clear winner.
5. Next step: compare engagement rate by posting hour, media type, traffic source and call-to-action to find what to post and when.

## Tools used
- Python, pandas, NumPy, Matplotlib, Seaborn
- Jupyter Notebook
- Antigravity IDE

## How to run
1. Download or clone this repository
2. Open the notebook in Antigravity IDE (or any Jupyter-compatible editor)
3. Install the libraries: `pip install pandas numpy matplotlib seaborn jupyter`
4. Change the CSV path in the notebook to where your dataset is saved
5. Run all cells
