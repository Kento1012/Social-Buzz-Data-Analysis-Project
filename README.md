## **Project Overview**
The Social Buzz project for Accenture involves analyzing datasets related to content types, reactions, and reaction scores using Excel. The goal is to identify the top five content categories with the highest audience engagement. The analysis includes data cleaning, integration, and visualizations such as pie charts and bar graphs to provide insights and recommendations for improving content strategy and audience engagement.



### <ins>Ask Phase</ins>

Situations and questions…

Accenture decided to start an initial 3-month project to expect 3 things. 
  1. Audit of their big data project
  2. Recommendation for successful IPO
  3. Analysis of content categories that highlight the top 5 categories with the largest aggregate people


### <ins>Prepare Phase</ins>
As a data analyst, I have to figure out the top 5 categories with the largest popularity from 3 data. 
  1. Content: This dataset contains entries for various types of content. It includes columns for the type of content (e.g., "photo," "video") and the associated category (e.g., "studying," "technology").
  2. Reactions: This dataset records reactions to the content. The type of reaction (e.g., "disgust," "interested"), and the date and time of each reaction.
  3. Reaction Types: This dataset categorizes each reaction type by its sentiment (positive or negative) and provides a score associated with each type, such as "heart" (positive, score 60) or "disgust" (negative, score 0).


### <ins>Process Phase</ins>
* Removed unnecessary columns:
  * Deleted User ID and URL as they did not contribute quantitative value to the analysis.
* Addressed missing data:
  * Deleted any blank entries in the Reaction Types table.
* Standardized formatting:
  * In the Content table...
    - Unified categories with and without quotation marks for consistency.
    - Converted all category names to lowercase for uniformity (using the LOWER() function).


### <ins>Analyze Phase</ins>
1. Set up base table:
  * Used the Reaction table as the primary dataset.
2. Joined content types:
  * Added Content Type information to the Reaction table using the VLOOKUP function.
3. Combined reaction scores:
  * Merged reaction scores from the Reaction Type table, aligning each reaction with its score.
4. Calculated total scores:
  * Applied the SUMIF function to calculate the total score of reactions for each category.

Here’s a concise summary of your dashboard components:
 * Pie Chart: Displays the top 5 categories by percentage, showing their share of the total.
 * Bar Chart: Shows the average reaction score per category, making it easy to identify which categories received the highest scores.
 * Line Graph with Pivot Table: Tracks the monthly count of each Reaction_Type by category. This focuses on the number of reactions (not scores) over time, providing insights into   engagement trends.

![Screenshot 2025-01-02 at 7 30 33 PM](https://github.com/user-attachments/assets/79c7f16a-7ae5-4f78-899c-697a1b497b75)

### <ins>Share Phase</ins>
With the Animal and Science categories dominating, <ins>there is potential to increase audience engagement by adding more category-focused content and continuing to capture existing interest. (So what)</ins>

When we focus on the response score in the five categories, the technology and healthy eating categories have higher average scores than the others, indicating that the audience favorably receives them. This suggests the potential for increased positive engagement.

<ins>It may be worth considering a strategy to further develop content related to the high-scoring categories to elicit positive responses and improve brand image and viewer loyalty. (So what)</ins>

<ins>The content distribution that follows seasonal trends, such as increasing content in related categories for specific times of the year, is expected to attract viewers at the right time and effectively increase engagement (So What). </ins>
