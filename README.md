This is a data scraping project using Python and the Beautiful Soup package to parse websites for video game, Pokemon, data.

The code was tested on a Jupyter Notebook and then uploaded to BitHub.

The code sets up a function that extracts all six of a Pokemon's stats, their name, ability, and number -- under different 7 different webpages on Serebii.com

The website makes some columns BOLD which caused Beautiful Soup to miss data when iterating through tags, so I had to create a function to iterate through the data and remove certain formatting tags <b> and </b>.

These tags also had a class = "fooben", which I had to iterate and change to have a "fooinfo" class so that Beautiful Soup can extract the information more precisely.

The code then parses through the webpages' html and extracts the data into a new list using the <td> tag and class = "fooinfo."

I then setup a function to iterate through the list and group the data further using a character's Pokemon Number. 

The code then saves the sublists into a csv file, and it iterates until all 7 webpages have been scraped, saving them to our desktop as well.

I was able to save and create 7 files that have the top 300 pokemon for stats - based on speed, defense, sp. def, sp. attack, hp, attack, overall stats.

The following is and example how the text is extracted (attached is the pokemon_stats_all.csv created from the "total stats" webpage):

#0493		Arceus		120	120	120	120	120	120


*****Please feel free to make any suggestions on how to optimize code****
