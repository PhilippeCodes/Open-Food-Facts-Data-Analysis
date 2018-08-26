# Open-Food-Facts-Data-Analysis-EPFL-Project-2-
Analyzing the Open Food Facts Dataset as Part of The EPFL Applied Machine Learning Course. The Purose of this Project is to exercise and demonstrate acquired Abilities. Should the Person who is looking at this Analysis have any Questions or Suggestions, do not hesitate to contact me.

## The Data
The actual file is too large (>1GB) in order to be added to this repository. However, it can easely be found and downloaded here: https://www.kaggle.com/openfoodfacts/world-food-facts/downloads/en.openfoodfacts.org.products.tsv/5
Open Food Facts is a non-profit association of volunteers. 5000+ contributors have added 600 000+ products from 150 countries.
The Dataset is a free, open, collbarative database of food products from all around the world, with ingredients, allergens, nutrition facts and information we can find on product labels.
The dataset contains a single table, FoodFacts, in CSV (TSV) form in FoodFacts.csv and in SQLite form in database.sqlite.
There are more than 300,000 rows over 163 columns. However, as we will see there are a lot of missing or obviously incorrect values.

fields that end with _t are dates in the UNIX timestamp format (number of seconds since Jan 1st 1970)
fields that end with _datetime are dates in the iso8601 format: yyyy-mm-ddThh:mn:ssZ
fields that end with _tags are comma-separated list of tags (e.g. categories_tags is the set of normalized tags computer from the categories field)
fields that end with a language 2 letter code (e.g. fr for French) is the set of tags in that language
fields that end with _100g correspond to the amount of a nutrient (in g, or kJ for energy) for 100 g or 100 ml of product
fields that end with _serving correspond to the amount of a nutrient (in g, or kJ for energy) for 1 serving of the product
nutrition-score-fr_100g : experimental nutrition score derived from the UK FSA score and adapted for the French market (these fields are of numeric, ranging from -15 to 40. The lower the score, the better)
nutrition-score-uk_100g : nutrition score defined by the UK Food Standards Administration (these fields are of numeric, ranging from -15 to 40. The lower the score, the better)
nutrition_grade_fr_100g : Seems to be a simple categorization of the score into A, B, C, D, and E (The UK equivalent contains mostly NaNs)

