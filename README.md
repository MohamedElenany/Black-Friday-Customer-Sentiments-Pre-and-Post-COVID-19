# Black-Friday-Customer-Sentiments-Pre-and-Post-COVID-19
## Main Objective
This project seeks to conduct an in-depth and quantitative analysis of the evolving sentiment scores related to Black Friday, specifically examining the period before and after the onset of the COVID-19 pandemic. The primary goal is to utilize advanced Natural Language Processing (NLP) techniques and regression analysis to unravel intricate patterns in consumer attitudes and behaviors during this crucial shopping event.

## Project Steps

### Data Retrieval & Pre-Processing
A diverse dataset comprising posts from subreddits such as amazonprime, blackfriday, bestbuy, anticonsumption, and walmart, totaling 49,309 posts, was collected. The data spans from 2018 to 2023, providing a comprehensive view of sentiments over multiple Black Friday events. The dataset underwent meticulous preprocessing, involving a comprehensive NLP pipeline encompassing tokenization, lemmatization, POS tagging, N-Gram modeling, and the application of Term Frequency-Inverse Document Frequency (TF-IDF).

### Sentiment Analysis
This project employs both VADER sentiment analysis and K-Means clustering methods to gain a comprehensive understanding of sentiment distribution within the dataset. The analysis revealed a nuanced breakdown of sentiments, with 26,002 posts classified as positive, 14,746 as neutral, and 8,561 as negative.

### Topic Identification (Latent Dirichlet Allocation - LDA)
To uncover latent topics within the textual data, a sophisticated Latent Dirichlet Allocation (LDA) model was implemented. The optimal configuration identified two topics, shedding light on distinct themes related to online and in-store shopping, with a balanced distribution of 47% and 53%, respectively.

### Logistic Regression Analysis
Employing logistic regression models on balanced datasets, sentiment predictions were made based on various features, including subreddit IDs, sentiment labels, comment scores, year information, and LDA results. Model performance was meticulously evaluated using accuracy, precision, recall, and F1 score metrics, with extracted coefficients providing insights into feature impact.

### Causal Inference Analysis (CausalML)
Causal inference analysis was conducted using the CausalML library to estimate the Average Treatment Effect (ATE) of the time period, treated as a binary treatment variable, on sentiment scores. Both T-learner (using gradient boosting) and S-learner (using linear regression) models were employed to quantify how sentiment scores are influenced by the transition from before to after the specified event, potentially COVID-19. ATE estimates suggested a slight decrease in sentiment scores following the event, indicating a potential negative impact on public sentiment as expressed in the analyzed text data.

## Results
The analysis revealed significant shifts in sentiments toward Black Friday, unveiling insights into evolving consumer behaviors and preferences. Notably, the sentiment toward online shopping exhibited a positive transition before COVID, culminating in a very positive sentiment after the pandemic. Conversely, sentiments concerning in-store shopping witnessed a decline post-COVID, signaling waning interest in the traditional in-store Black Friday experience. The study also highlighted a noteworthy shift in the perception of Black Friday as a dedicated shopping day, evidenced by a substantial decrease in the average number of Reddit posts during Black Friday periods after COVID, indicating a diminishing enthusiasm for the event.

Anticonsumption sentiments followed a positive trajectory, transitioning from a stance of despising anticonsumption to a more restrained approach. This shift may be influenced by factors such as inflation and changing consumer attitudes. Additionally, a retailer-specific analysis underscored divergent sentiments toward major players. Amazon and Best Buy experienced improved post-COVID sentiments, attributed to their concerted efforts in enhancing the online shopping experience. In contrast, Walmart faced more negative sentiments, potentially reflecting perceived shortcomings in adapting to the evolving online shopping landscape.

## Applicability and Business Value of Results

The project's findings carry significant implications for businesses, offering actionable insights into evolving consumer sentiments with direct relevance to marketing, inventory management, and customer experience strategies. Notably, the observed positive shift in sentiment toward online shopping and the decrease in enthusiasm for in-store Black Friday experiences post-COVID underscore the changing landscape of consumer preferences. This information equips businesses with the knowledge to adapt their marketing efforts, focusing more on online channels and reevaluating the traditional in-store Black Friday approach.

Economically, the project provides valuable intelligence for decision-makers. Understanding the subtle nuances in sentiment before and after the pandemic aids businesses in forecasting consumer behavior, guiding pricing strategies, and optimizing inventory to align with shifting preferences. This can contribute to increased efficiency in resource allocation and enhanced decision-making processes, ultimately impacting the bottom line positively.

Societally, the findings contribute to ongoing discussions on consumption patterns and sustainability. The positive trend in anticonsumption sentiments indicates a potential shift in consumer attitudes towards more mindful and restrained consumption, possibly influenced by factors such as inflation. This societal shift has broader implications for businesses and policymakers as they navigate the evolving landscape of consumer expectations and values.

In conclusion, the project's results provide actionable insights that extend beyond the realm of sentiment analysis, offering a strategic guide for businesses to navigate the evolving consumer landscape effectively.




