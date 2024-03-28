This is a data scraping project using Python and the Beautiful Soup package to parse websites for video game, Pokemon, data.

The code sets up a function that extracts all six stats for Pokemon and their name, under different webpages for viewing Top Stats (i.e. speed, defense, sp. attack, etc...) on the Serebii's website.

The website makes some columns BOLD which caused Beautiful Soup to miss data, so I had to iterate through the data and remove certain formatting tags.

The code parses through the websites html and extracts the data into a new list.

I then setup a function to iterate through the listen and group the data by character using their Pokemon Number (Pokemon).

The code then saves the sublists into a csv file, and it iterates until all 7 webpages have been scraped, saving them as to our desktop as well.

I was able to save and create 7 files that has their respective top 300 pokemon  based on speed, defense, sp. def, sp. attack, hp, attack,overall stats, their name and number.


