Example Flows:

Douglas, a casual player, has taken an interest in the Plague Doctor role and wants to find and save a script that includes the Plague Doctor but is also balanced for his inexperienced group of players. First, he'll nedd to create a specific search for all scripts that include the Plague Doctor. Given the selection, he'll then need to select a couple of them to see the full character lists and choose his favorite. For each of those, he'll need to create compositions and collect average win rates for the script given a random selection.
To do so, he needs to:
 - Call GET /scripts and pass in a parameter filtering for Plague Doctor. Lets say one of the displayed scripts is a script with ID 138.
 - Call GET /scripts/138 and examine the full character list and author description.
 - Call POST /compositions and specify the script and the chosen characters, creating a composition with an ID 12.
 - Call POST /compositions/12/stats to return the average game stats.
 - Call GET /scripts/138/download which downloads the script to his computer.

Randal, an expierenced player, wants to keep track of all the scripts of characters/roles he's played so far by how good they are. The best way to do that is giving them ratings so that next time he plays, he'll pick the script with the best ratings, or maybe the lowest ratings if he wants to go easy on new players. First, he'll search for the scripts he's played with, then rate them
- Call GET /scripts and put in the ID for the script he's previously played with. Let's say the character he's played before is Monk, and it's character ID is 125
- Call GET/ scripts/125 to pull up the character listings
- Call POST /scripts/125/rate and gives a rating to the Monk
- Repeat process with other roles he's played with

Bobby, an ethusiastic script writer, wants all his written scripts to be stored in a database. He wants to give them a unique name so that he can access them them depending on the situation.
Bobby want to create a script name "Spooky", with a list of 5 ghost characters. After a while he wanted to add a description to his script. 
- Call GET scripts/ "Spooky" to make sure your script has a unique name. 
- Call POST /scripts/add and in all info. Lets assume this is the first script"Spooky", [Boo, Casp, Shro, Poka, Low]
- Call PUT /script/1/edit Here a scary description will be added to the Spooky script
  
