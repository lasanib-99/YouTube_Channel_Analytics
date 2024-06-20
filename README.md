# YouTube Channel Analytics
Power BI Project analyzing the statistics of the most subscribed YouTube channels to uncover key success factors.

## Research Problem:
What factors contribute most to the earnings of top YouTube channels, and how do these factors vary across different types of channels and countries?

## 'Global YouTube Statistics' Dataset:

### Variable Description: 

- `rank`: Position of the YouTube channel based on the number of subscribers
- `Youtuber`: Name of the YouTube channel
- `subscribers`: Number of subscribers to the channel
- `video views`: Total views across all videos on the channel
- `category`: Category or niche of the channel
- `Title`: Title of the YouTube channel
- `uploads`: Total number of videos uploaded on the channel
- `Country`: Country where the YouTube channel originates
- `Abbreviation`: Abbreviation of the country
- `channel_type`: Type of the YouTube channel (e.g., individual, brand)
- `video_views_rank`: Ranking of the channel based on total video views
- `country_rank`: Ranking of the channel based on the number of subscribers within its country
- `channel_type_rank`: Ranking of the channel based on its type (individual or brand)
- `video_views_for_the_last_30_days`: Total video views in the last 30 days
- `lowest_monthly_earnings`: Lowest estimated monthly earnings from the channel
- `highest_monthly_earnings`: Highest estimated monthly earnings from the channel
- `lowest_yearly_earnings`: Lowest estimated yearly earnings from the channel
- `highest_yearly_earnings`: Highest estimated yearly earnings from the channel
- `subscribers_for_last_30_days`: Number of new subscribers gained in the last 30 days
- `created_year`: Year when the YouTube channel was created
- `created_month`: Month when the YouTube channel was created
- `created_date`: Exact date of the YouTube channel's creation
- `Gross tertiary education enrollment (%)`: Percentage of the population enrolled in tertiary education in the country
- `Population`: Total population of the country
- `Unemployment rate`: Unemployment rate in the country
- `Urban_population`: Percentage of the population living in urban areas
- `Latitude`: Latitude coordinate of the country's location
- `Longitude`: Longitude coordinate of the country's location

### Preprocessing
- **Total observations:** 864 out of 995
- **Removed unnecessary rows:** Removed 5 observations where the columns of `created_year` and `created_date` had errors 
  - `video_views_for_the_last_30_days` changed to whole number after changing ‘nan’ values to ‘0’
  - `subscribers_for_last_30_days` changed to whole number after changing ‘nan’ values to ‘0’
  - `created_year` changed to “text”
- **Removed unnecessary columns:**
  - `Rank`, `Title`, `Abbreviation`, `Category`, `lowest_yearly_earnings`, `highest_yearly_earnings`, `created_date`, `Population`, `Unemployment rate`, `Latitude`, `Longitude`, `Urban_population`
- **Imputing with missing values:**
  - `Country` replaced with “United States” - mode
  - `Channel_type` replaced with “Entertainment” – mode
  - `video_views_for_the_last_30_days` replaced with “165726691” - mean
  - `Gross tertiary education enrollment (%)` replaced with “55.8” - mean
 
## Objectives of the Study
### Targeting both YouTube content creators and the Managerial level

- Gain valuable insights into the success factors of top YouTube channels and understand what sets them apart from the rest.
- Discover the most popular categories and upload frequencies that resonate with audiences.
- Identify influential YouTube creators from different countries and analyze their impact on a global scale.
- Explore the correlation between channel performance such as uploads, views, subscribers and estimated earnings.
- Visualize the distribution of successful YouTube channels on a world map and uncover geographical trends.

## Key Insights Obtained

- **Entertainment and Music** channel types are the most popular.
- Channels focused on popular topics like entertainment, music, and gaming tend to attract larger audiences and advertisers, resulting in higher earnings.
- Channels with a large and engaged audience tend to earn more (subscribers, views, uploads).
- Regularly uploading new content can help channels maintain audience interest, improve visibility in YouTube's algorithm, and increase overall watch time.
- A large subscriber base indicates a loyal audience that is likely to engage with the channel's content and leads to higher earnings.

## How to Use

1. Clone this repository to your local machine using Git.
git clone
2. Explore the Analysis 'Youtube_Metrics.pbix' to understand the data processing and visualization.
