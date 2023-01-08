# Big-Data-Analytics
## SI 699 - Capstone Project: Biased Restaurant Reviews: Starbucks in NYC

### Introduction
In recent years, online customer reviews or product reviews have become the major source for collecting feedback from customers. Restaurant owners could find ways to improve their service or even evaluate whether a new store is easy/hard to gain good ratings and reviews in a specific location by analyzing those online reviews. In this project, we want to explore the factors that cause regional bias in restaurants’ ratings. We chose Starbucks as the target store to analyze since it is our favorite and the most popular chain store in U.S.A. We are curious about why the same brand with almost the same products could receive different ratings in different locations.
The analysis will first focus on boroughs in New York City due to the time limit and the project scope. By analyzing the online review text with regional data (i.e. income levels) of Starbucks in different regions, we want to answer the following two questions:
1. What factors do customers care about Starbucks?
2. If those factors varied by region? If so, do income levels make them different?
The analysis result of this case study will provide the business owners the insight into how to satisfy the customers and run a business successfully in each region.

### Methods
To understand the customers’ reviews and the related sentiment towards certain aspects of Starbucks, we implemented two models and Correlation Analysis:
* Aspect Extractor: extract the opinion aspects and polarity from each review sentence
* Aspect Classifier: classify the aspects for further analysis

### Conclusion and discussion
Overall, for NYC specifically, although the ratings of Starbucks are only 4% higher in low income regions, according to our literacutre review, this might be because business owners might spot an opportunity to gain customers by improving their customer service, especially in low income areas. In addition, patrons living in low income neighborhoods would have the ammunition to demand better customer service in the restaurants they frequent. And city hall officials might also see this as a form of income segregation and work harder to ensure restaurants in low income areas have the same amenities and service levels as those in middle or high income areas. However, we did not see a strong relationship between reviews and income levels.

### Limitations
* We’ve made an assumption that customers going to Starbucks have the same demographic
distribution as the local citizens. However, this assumption doesn’t necessarily
hold. The main target segment of Starbucks customers aged from 25 to 40 with high
incomes, and the second target group is 18 to 24 years of age and belongs to richer families.
11 We made this assumption because the actual customers’ information is unavailable
due to privacy policy. Real customers’ information will give more reasonable results in the
correlation analysis.
* The aspect extractor is trained on the SemEval-14 restaurant review dataset. The distribution
may differ from our dataset. The accuracy of the aspect extractor will largely affect
the ad hoc analysis.
* The aspect classification is done by using unsupervised methods. We still need to manually
identify the meaning of each cluster. We also don’t have control over the level of
granularity that how these aspects are classified.
* Due to the limited availability of demographic information, we mainly focus on Starbucks
near NYC. The findings may or may not be applied to other coffee shops or regions.
* The data points are not sufficient to understand customers’ preferences in different areas.
General aspect words take up to 40% of our categories, e.g. “coffee” for the coffee
category.

### References
[1] Lian, J.; Zhang, F.; Xie, X.; Sun, G. Proceedings of the 26th International Conference on World Wide Web Companion; WWW ’17 Companion; International World Wide Web Conferences Steering Committee: Republic and Canton of Geneva, CHE, 2017; p 993–1002.

[2] Muchnik, L.; Aral, S.; Taylor, S. Social Influence Bias: A Randomized Experiment. Science (New York, N.Y.) 2013, 341, 647–51.

[3] Mbuthia, J. Is there a correlation between a restaurants ratings and the income levels of a neighborhood? (August 2019); https://medium.com/swlh/is-there-a-correlation-between-a-restaurantsratings- and-the-income-levels-of-a-neighborhood-5fe41165e4f1.

[4] Hossain, N.; Bhuiyan, M. R.; Tumpa, Z. N.; Hossain, S. A. Sentiment Analysis of Restaurant Reviews using Combined CNN-LSTM. 2020 11th International Conference on Computing, Communication and Networking Technologies (ICCCNT). 2020; pp 1–5.

[5] Yang, H.; Zeng, B.; Yang, J.; Song, Y.; Xu, R. A multi-task learning model for Chinese-oriented aspect polarity classification and aspect term extraction. Neurocomputing 2021, 419, 344–356.

[6] Jurafsky, D.; Chahuneau, V.; Routledge, B.; Smith, N. Narrative framing of consumer sentiment in online restaurant reviews. First Monday 2014, 19.

[7] Octoparse. https://www.octoparse.com/.

[8] Miller, G. A. WordNet: a lexical database for English. Communications of the ACM 1995, 38, 39–41.

[9] Yang, H.; Li, K. PyABSA: Open Framework for Aspect-based Sentiment Analysis. 2022; https://arxiv.org/abs/2208.01368.

[10] Sculley, D. Web-scale k-means clustering. Proceedings of the 19th international conference on World wide web. 2010; pp 1177–1178.

[11] Haskova, K., et al. Starbucks marketing analysis. CRIS-Bulletin of the Centre for Research and Interdisciplinary Study 2015, 1, 11–29.
