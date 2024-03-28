This is a data scraping project using Python and the Beautiful Soup package to parse websites for video game, Pokemon, data.

The code sets up a function that extracts all six of a Pokemon's stats, their name, ability, and number, under different 7 different webpages on Serebii.com

The website makes some columns BOLD which caused Beautiful Soup to miss data, so I had to iterate through the data and remove certain formatting tags <b> and </b>.

These tags also had a class = "fooben" which I had to iterate and change to have a "fooinfo" class so Beautiful Soup can extract the information more precisely.

The code parses through the websites html and extracts the data into a new list using the <td> tag and class = "fooinfo."

I then setup a function to iterate through the list and group the data further using a character's Pokemon Number. 

The code then saves the sublists into a csv file, and it iterates until all 7 webpages have been scraped, saving them to our desktop as well.

I was able to save and create 7 files that have the top 300 pokemon for stats - based on speed, defense, sp. def, sp. attack, hp, attack, overall stats.

The following is and example how the text is extracted:

#0493		Arceus		120	120	120	120	120	120


