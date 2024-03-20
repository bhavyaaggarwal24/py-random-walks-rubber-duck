# Python code for rubber ducks floating down a canal being affected by the current and wind

This is a simple model of the real world using Random Walks. A rubber duck has been considered floating down a canal being affected by the current and wind. 

Fisrt class is current whose initialization method gives an initial velocity and direction which will default to 0 degrees (due north.) A method called get_vector() returns the current velocity and direction. Each time get_vector() is called the velocity will randomly change in the range of 0.5 to 2.0 and the direction will change 5 degrees. (The velocity will be feet per iteration.) 

Location class is to track the location of an object, and a class called Canal to hold our rubber ducks, it also has a width. Current is an attribute of the canal.  If an object hits the bank the vector will reflect off of the bank - that is if the direction is 45 degrees the reflection would be 135 degrees. 

Duck class is created to hold our duck racers. The take_step method adds two current vectors, one for the canal and the other for the wind, together to determine the impact of that step.

"run_race" function takes three parameter; the number of ducks, the width of the canal, and the length of the race. Race starts by placing the ducks next to one another in the middle of the canal. Then ducks moves until one crosses or completes the length of the race. Each iteration gets the vector for the canal as well as a vector for the wind. Those two parameters are being provided to each duck as they move down the canal. 

When the first duck completes the race rank all the ducks based on how close they are to the finish (closest is second, and so on.) A graph is created showing the progress of each duck.

The subclass of Current called Wind has been created which models some additional random behavior. 5% of the time the wind can change direction in the range of 15 to 20 degrees and 1% of the time will gust an addition 20 feet per iteration and will last 3 iterations.

 A graph is created showing the progress of each duck and ranking of the duck displayed :) 

