README.txt

# Four Zero Project

CS230 Software Development Project for Swansea University, group 40.

Background Gif for menus sourced from here: http://bestanimations.com/Nature/Flora/Trees/forest-trees-animated-gif-15.gif

Pathing algorithm explanation:

The asset system that the game uses, for paths uses binary naming standards to show what would be around the cell theoretically on the map. 
The implementation checks for surrounding cells that are Walls and aren’t Walls (not to be confused with Paths) 
– this is because it could be a teleporter, goal, log or boulder and checking for not Walls is more inclusive than checking for just Paths. 

The algorithm checks for the number and orientation of Walls around the centre cell that have an x or y value of zero. 
It then looks at the corners in the algorithm to determine the texture applied. 

The algorithm also maps images for other cells being Walls, Teleporters, Goals, Boulders, Logs, Water and Lava. 
It uses a checking system to check the surrounding cells, but due to placement restrictions the conditions it checks are a lot move limited than Path assignment.  
However, for Walls it randomly assigns a wall image that is stored in assets to make the game more aesthetically pleasing. 


Compling Instructions:

All the code needed to run FourZero is provided in the src file in submission. This includes the assets, .txt files for leaderboards
and profiles as well as the code.

Compiling and running the code should be fairly simple, if for some reason it does fail,
ensure the .txt files (leaderboard folder and profilesFile.txt) are blank and try again.