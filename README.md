# Yelp-Chicago-Eats
#python #api #tableau #webscraping #data cleaning #requests #pandas #requests #json #shapefile

<iframe src="https://public.tableau.com/views/BestEatsinChicagoNeighborhoods-Yelp/Sheet2?:embed=y&:display_count=yes"
 width="645" height="955"></iframe>

I began this project with a few question in mind...

Where do I go in Chicago for the best (cajun) food? What type of food is a neighborhood known for?

In order to create this, I imagined the final product to be a tableau visualization where I would be able to filter by type of food and visualize the ranking of neighborhoods by that type. I'd also be able to see that xyz neighborhood is known for bagels etc.

## Final Steps
1. Build list of Chicago neighborhoods from shapefile
2. Search the Yelp API for all restaurants in the list of neighborhoods
3. Separate the data into each category per row
4. Export shapefile and csv to Tableau
5. Build a geo visualization by weighted score and filter by category

Prior to finalizing this project, I had to undergo multiple levels of exploration. Initially I was looking for a convenient way to grab all the neighborhoods in Chicago, but was unable to find an easy transferable source. Then, I decided to utilizing webscraping on wikipedia's page of chicago communities using the beautifulsoup package. After pulling the data and running the api in yelp, it still pulled out several holes in the visualization when ran with the shapefile. Fortunately, the shapefile came with a ready list of neighborhoods in Chicago. All that was needed was to read the shapefile in python and pull the list of neighborhoods out of to run on the yelp api.
