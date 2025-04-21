API Specifications:
Script Listing Page
1.1. List/Search scripts - /listing/search/ (READ)
	Displays the generic search page for all of the listings, and also be able to be applied to only return specific a specific listing based on search parameters. Just listing every available script should require no parameters. 
1.2. Add a new script to database - /listing/add/ (WRITE)
  Creates a new script in the database with a unique id, name, character list, and (optional) text description. 
1.3. Edit an existing script - /listing/edit/ (WRITE)
  Lets you change the name, character list, or description of a given script.
1.4. Rate script - /listing/rate/ (WRITE)
  On the listing page, all of the scripts will have a rating attribute. This can increment or decrement the total by one. 
1.5. Select script to examine - /listing/examine/ (READ)
  On the main listing page, the descriptions and full character lists aren't going to be visible. By examining, the user should be able to go into a different page that displays the relevant information about that script and allows them to directly access the script compostion tool from there.
1.6. Download script - /listing/download/ (READ)
  Downloads a text file containing the characters and name of the script, to import and use on other sites.

Script Compostion Tool
2.1. Create a composition of available characters - /script/choose/ (WRITE)
  Selects a specific amount of characters from a given list and saves them as a composition (in a new table) that can be accessed by the other commands.
2.2. Run step-by-step example game with AI - /script/runwithai/ (READ)
  Creates and runs through a step-by-step user interface to guide them through an example game that produces logs.
2.3. Collect average win rate and stats by running many games with AI - /script/stats/ (READ)
  Runs a user-defined amount of random games automatically, collecting cumulative data on win and death rates and returning them to the user.
