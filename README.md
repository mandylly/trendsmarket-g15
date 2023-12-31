#  MSBA6331-Simplifying Recommender Systems: Amazon Personalize x Amazon SageMaker Data Wrangler
This work is completed in partial fulfillment of the requirements for the Big Data Analytics course offered by the Master of Science in Business Analytics program at the Carlson School of Management, University of Minnesota.

## Project Overview
The project aims at unlocking the synergy of Amazon Personalize and Amazon SageMaker Data Wrangler. Amazon Personalize has been the go-to recommendation tool as it integrates multiple algorithms into a single platform. It is especially valuable to small businesses that may not have the resources to develop their proprietary recommendation systems. On the other hand, Amazon SageMaker Data Wrangler makes data pre-processing extremely simpler as it contains over 300 built-in data transformations, so one can quickly transform data without writing any code and complete each step of the data preparation workflow (including data selection, cleansing, exploration, visualization, and processing at scale) from a single visual interface. We intend to use both these tools to showcase the potential of Amazon Personalize in a very user-friendly way without the need for writing tonnes of code. We will also evaluate the efficacy of different recommender systems in comparison to Amazon Personalize.

## Business Problem
Recommender systems are crucial in establishing a strong relationship with a consumer to the subscription service or e-commerce platform that they opt for. We see strong recommender systems being in action when we shop online (Walmart), watch movies (Netflix, Hulu), music streaming platforms (Spotify) etc. While these corporate giants can afford to have a data science team that will help them with the data pre-processing and feature engineering steps before the recommender system steps in, small business owners still struggle to use the same. This is where Amazon SageMaker Data Wrangler and Personalize can empower small businesses with limited capacity and resources to develop recommender systems for their businesses without needing the skills of a seasoned data scientist.

## Quick Links
[Flyer](https://github.com/mandylly/trendsmarket-g15/blob/0ca67b06d24f14d756dbf4ac5d1dafc2e55e3d7b/Trends%20-%20Fall'23%20-%20G15.pdf)

[Project Video](https://www.youtube.com/watch?v=nH8Fcw-tWBU)

[Slides](https://github.com/mandylly/trendsmarket-g15/blob/7a6222418a109f7aeec64f8a39dcdbe342aa768c/Slides.pdf)


## Dataset Resource
Movie: 
https://grouplens.org/datasets/movielens/

Books Recommendation: 
https://www.kaggle.com/datasets/arashnic/book-recommendation-dataset?select=Ratings.csv

Beer: 
https://www.kaggle.com/datasets/thedevastator/1-5-million-beer-reviews-from-beer-advocate/data

## Getting Started
To utilize AWS SageMaker Data Wrangler and AWS Personalize for your data analytics and personalization projects, please follow the setup instructions below.

### Prerequisites
An AWS account with access to SageMaker and Personalize.
Basic understanding of data processing and machine learning concepts.
Familiarity with Jupyter notebooks.

### Installation and Setup
#### Use Data Wrangler
1. Choose the dataset group that you create

2. Choose the data set you are going to import

3. Choose data wrangler as import method

4. Import data to data wrangler

5. Start transform your data by “Add Step”

6. Export the data to S3 bucket

Here is a link for the guide: [datawrangler_guide](https://github.com/mandylly/trendsmarket-g15/blob/1b33453412d3ebbe4adddd62e2fe624903eb18c7/datawrangler_guide.ipynb)

<img width="1255" alt="image" src="https://github.com/mandylly/trendsmarket-g15/assets/152313718/e9b668e5-3f6f-4c98-a691-a27227b99608">

#### Use Personalize
1. Initiate the process by navigating to the Amazon Personalize console and establish a new dataset group.

2. The dataset group consists of three distinct domains: E-commerce, Video on Demand, and Custom. Make a selection based on the characteristics of your dataset.

3. Upon successful creation of a dataset group, proceed to create individual datasets within the group. This includes the mandatory user interaction dataset, as well as optional item and user datasets.

4. Move forward to create a solution within the dataset group, carefully selecting an appropriate recipe. 

5. A recipe serves as the foundational framework for the machine learning model, streamlining the complexities involved in model construction and training to facilitate the generation of personalized recommendations.

6. Subsequently, upon the creation of a recipe, input the relevant item and user identifiers to obtain personalized recommendations, tailoring the output to the specific characteristics of the dataset and recommendation use case.
![product-page-diagram_Amazon-Personalize1 4249579be4fd5c883914489dcbb0c27ba59a2961](https://github.com/mandylly/trendsmarket-g15/assets/152313718/cee94e62-4489-4cac-827c-05c6b3f5bbac)


## Use Cases
#### Tailored News Feed: 
For a news platform, Amazon Personalize can curate a personalized news feed based on user interaction history, keeping readers engaged and increasing time spent on the platform.

#### Customized Travel Recommendations: 
A travel site can use Amazon Personalize to offer hotel, flight, and excursion recommendations based on previous bookings and searches, enhancing the booking experience.

#### Personalized Learning Paths: 
An e-learning platform can leverage Amazon Personalize to suggest courses and materials tailored to the learner's progress and interests, improving learning outcomes.

## Bibliography and Credits
[Trending-Now-Recipe](https://docs.aws.amazon.com/personalize/latest/dg/native-recipe-trending-now.html)

https://aws.amazon.com/personalize/

https://aws.amazon.com/sagemaker/data-wrangler/

https://www.youtube.com/watch?v=3gJmhoLaLIo&list=PLLNv7WFv3KhiulXWUjPy-RgPGjSi338gL&index=2

https://docs.aws.amazon.com/personalize/latest/dg/creating-recommenders.html

https://aws.amazon.com/blogs/architecture/architecting-near-real-time-personalized-recommendations-with-amazon-personalize/

https://github.com/aws-samples/amazon-personalize-samples/blob/master/next_steps/core_use_cases/trending_now/

https://github.com/aws-samples/amazon-personalize-samples/tree/master/next_steps/core_use_cases/personalized_ranking



