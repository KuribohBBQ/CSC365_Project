Example Flows:

Douglas, a casual player, has taken an interest in the Plague Doctor role and wants to find and save a script that includes the Plague Doctor but is also balanced for his inexperienced group of players. First, he'll nedd to create a specific search for all scripts that include the Plague Doctor. Given the selection, he'll then need to select a couple of them to see the full character lists and choose his favorite. For each of those, he'll need to create compositions and collect average win rates for the script given a random selection.
To do so, he needs to:
 - Call GET /scripts and pass in a parameter filtering for Plague Doctor. Lets say one of the displayed scripts is a script with ID 138.
 - Call GET /scripts/138 and examine the full character list and author description.
 - Call POST /compositions and specify the script and the chosen characters, creating a composition with an ID 12.
 - Call POST /compositions/12/stats to return the average game stats.
 - Call GET /scripts/138/download which downloads the script to his computer.


