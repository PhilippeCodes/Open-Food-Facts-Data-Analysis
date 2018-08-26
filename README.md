# Open-Food-Facts-Data-Analysis-EPFL-Project-2-
We will be analyzing the Open Food Facts Dataset as Part of The EPFL Applied Machine Learning Course. The purpose of this project is to exercise and demonstrate acquired abilities. Should the person who is looking at this analysis have any questions or suggestions, do not hesitate to contact me.

## The Data
The actual file is too large (>1GB) in order to be added to this repository. However, it can easily be found and downloaded here: https://www.kaggle.com/openfoodfacts/world-food-facts/downloads/en.openfoodfacts.org.products.tsv/5 <br>
Open Food Facts is a non-profit association of volunteers. 5000+ contributors have added 600 000+ products from 150 countries.
The Dataset is a free, open, collaborative database of food products from all around the world, with ingredients, allergens, nutrition facts and information we can find on product labels.
The dataset contains a single table, FoodFacts, in CSV (TSV) form in FoodFacts.csv and in SQLite form in database.sqlite.
There are more than 300,000 rows over 163 columns. However, as we will see there are a lot of missing or obviously incorrect values.

## Data Wrangling

We will take a closer look at our data and eliminate all columns that are either (mostly) empty or irrelevant for our investigation.
We will also get rid of any duplicates in our data. We will subsequently try to bring the remaining data in a more useful format and clean up any invalid entries. We will use the "serving_size" column to try to extract information on whether the product is liquid or solid.

## Exploration/Investigation

In the first half of our investigation we will primarily focus and on the following three areas:
- Frequencies (how are our variables distributed and what are the most common additives and ingredients?)
- Characteristics (what are the characteristics of the different categories and countries?)
- Relationships (how are the variables related to each other)

We will subsequently investigate our data with correlations and regression analysis.

We will finish this project by summarizing our findings
