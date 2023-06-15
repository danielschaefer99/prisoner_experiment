# Prisoner Experiment
Implementation of the Prisoner Experiment as seen in Veritasium video: https://www.youtube.com/watch?v=iSNsgj1OCLA

Starting point:
	100 prisoners numbered 1-100
	Slips with their numbers are randomly placed in 100 boxes in a room
	Each prisoner may enter the room one at a time and check 50 boxes
	They must leave the room exactly as they found it and can't communicate with the others after
	If all 100 prisoners find their number during their turn in the room, they will all be freed. But even if one fails, they will all be executed.
	What is their best strategy?

Implements:
	a random pick function, where prisoners pick 50 random boxes
	a circular pick function, where prisoners first pick the box with the label corresponding to their number and then repeatedly the box with the label of the number contained in the previous box
	
Number of runs and number of prisoners can be modified as global variables.

Outputs:
	The number of successful runs (Runs where ALL prisoners managed to find their number)
	The success chance relating to the number of runs performed
	The success chance of the individual prisoners
