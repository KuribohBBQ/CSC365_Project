User Stories:
1. As a professional gamer, gambler, and statistician, I want to examine the statistics and win rates of various roles so that I can know the odds of victory at all times.
2. As a game master with too little time to prepare, I want to run a very quick simulation of the script I am going to run so that I can check for any last-minute blindspots. 
3. As a game master for a group of players that consistently lose to the evil team, I want to find a script that has the odds favored for the good team so that the game is balanced.
4. As a script writer, I want to see how the addition of a character (such as the Slayer) to my custom script can alter the balance of the game so that I can decide whether to actually implement it or not.
5. As a social and humorous gamer, I want to create ridiculous and otherwise impossible scenarios and memes within the system so that I can humor myself and my friends.
6. As an experimental and inventive game designer, I want to see how far I can push the limits of the system in hopes of creating a completely unrecognizable and new but still playable and entertaining experience.
7. As a strategic player, I want to compare the win rates of my in-person group and the AI simulation of the same scripts so that I can see if a random-choice strategy is viable.
8. As a sandbox gamer, I want to watch the AI play games for me so that I can enjoy the (completely simulated) hijinx of (not) social deduction as a spectator.
9. As an enthusiastic script writer, I want to store my various scripts and variations in a database so that I always have the correct one for a given group or occasion.
10. As a lover of instigating my friends into raging and crashing out, I want to easily able to create chaotic scenarios that will turn my friends into quality content to watch
11. As a someone who plays RPGs a lot, I want a system that organizes the countless variables of a characters into tables so that it is easy to read
12. As an unexperienced player, I want to remain passive so that I can stay in the game for a longer time. 

Possible Exception Cases:
1. If a user tries to run a game with more/fewer roles put in than the amount of AI players, then the interface will give an error back to the user and prompt them to remove/add roles.
2. If a user tries to run a game with either an invalid script or none at all, the interface will give back an error because it won't be able to run the simulation.
3. If a user submits a script that does not at least have 1 listed demon, then the interface will give back an error prompting the user to submit a script that has a win condition for the good team.
4. If a user tries to run a game without selecting a demon role to be distributed, then the interface will prompt an error and request the user to add a demon.
5. If a user submits a script that has a role that either doesn't exist or is not implemented, the script editor will return an error and prompt the user to make a different choice.
6. If a user tries to add the same role to a script twice, the script editor will check to see if the role already exists and either return an error or refuse to make the change.
7. If a user tries to run a game with a valid script but too many bots to distribute unique roles to, then the game will prompt the player to add less bots.
8. If an unhandled exception causes a simulated game to take too long/never end, the game will end itself and return an error.
9. If an AI is put in a situation to make a choice/action it is unable to do, the game will end and return an error.
10. If an AI is assigned two contradictory roles, the interface will query the user to pick only one.
11. If both teams achieve their win conditions simultaneously, the game will probably return an error. Or a draw, if properly handled.
12. If a user tries to edit a script while a corresponding game is running, the game will probably end abruptly and return an error.
