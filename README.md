# Buy Sight: Sentiment Analysis on Products

## Abstract

Product specifications alone do not provide users with a comprehensive understanding of a specific product. Product reviews are crucial in making informed purchasing decisions, but analyzing a large volume of customer feedback manually can be cumbersome. Our solution involves implementing sentiment analysis on product reviews, grouping them based on their specifications/aspects. Users can search for desired products along with specific features, and based on previous customer reviews, they will receive recommendations for products from brands that align with their preferences.

## Description

Users input the desired product and feature, from which we generate an Amazon URL and randomly select three products. We scrape product reviews from Amazon using Octoparse, producing a CSV file. The CSV file contains various fields, with the review body being the input to our model. We preprocess the data by removing stop words, numbers, special characters, and white spaces using regular expressions. Each review is assigned a sentiment score based on its positivity, negativity, or neutrality. We tokenize words, assign POS tags, and handle phrases like 'not bad' to improve interpretation. The majority sentiment (negative, positive, neutral) is assigned to each product. The model processes data from three products to determine the best choice.

## Modules Used

- Pandas
- Matplotlib
- Regular Expression (re)
- NLTK
- Wordcloud

## Screenshots

<img src="https://github.com/nirmaljoji/BuySight/assets/40449660/3c67913d-8008-4734-8c3f-8770a1d33c2c" width="500" />

<img src="https://github.com/nirmaljoji/BuySight/assets/40449660/80d92ee2-4759-4a90-9637-43a84a9a64b9" width="500" />

<img src="https://github.com/nirmaljoji/BuySight/assets/40449660/657e34a1-6d4a-4526-ac29-4b727b4473cf" width="500" />

<img src="https://github.com/nirmaljoji/BuySight/assets/40449660/efe003e9-c4f8-446f-8a1e-47f035f13b1f" width="500" />
