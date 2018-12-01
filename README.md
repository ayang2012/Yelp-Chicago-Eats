# Yelp-Chicago-Eats
#python #api #tableau #webscraping #data cleaning #requests #pandas #requests #json #shapefile

<div class='tableauPlaceholder' id='viz1543637760386' style='position: relative'><noscript><a href='https:&#47;&#47;github.com&#47;ayang2012&#47;Yelp-Chicago-Eats'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Be&#47;BestEatsinChicagoNeighborhoods-Yelp&#47;Sheet2&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='BestEatsinChicagoNeighborhoods-Yelp&#47;Sheet2' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Be&#47;BestEatsinChicagoNeighborhoods-Yelp&#47;Sheet2&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1543637760386');                    var vizElement = divElement.getElementsByTagName('object')[0];                    vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>

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
