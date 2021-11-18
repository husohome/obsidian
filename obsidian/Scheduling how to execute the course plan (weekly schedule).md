# Scheduling how to execute the course plan (weekly schedule)

> this is part of the [[java project - productivity bookkeeper]] project.
#java #coding #productivity #productivity-book-keeper #project


## UI components
there are maybe three essential UI components (boxes) in this view (and you should add breadcrumbs of course)
1. course tracker box: 
		- courses and credits set according to the plan (in cards)
		- then you can drag and drop the courses to the scheduler box,
			- each time you drop a "course" to the scheduler box, it triggers the following things
				- it asks you how many credits (from 1 to max, which is the set credit for the course) to plan in a time
					- once you choose the number of credits, that many credits are set to the scheduled time in the weekly scheduler box.
					- the corresponding course card from the course reduces that many credits from it.
2. weekly scheduler box: 
		- is a schedule, like a google calendar (maybe even provide some integration? don't attempt for now)
		- you drag courses from the course tracker box,
			- of course, if you right click the box,
				- there should be a "cancel" option (to return the scheduled credit back to the credit)
					- it would be great if there's a transition animation
				- then, maybe an option to make it recurring (don't work on this yet)
	- You actually need to "commit" to the weekly schedule to sort of save it
		- there should be a warning that once committed, you'll can't change it
			- and they choose "I understand"

## Data validation
- happens before committing, obviously
- checks if you've used up all the course credits
- 

## other "considerate" features
- allow users to maybe right click the course card
		- directly edit the card,
			- can edit name, description, and adjust hours
		- sync back with the both
			- course plan
			- the "unique course" collection


## What users do action-wise
- drag the "course cards" from the tracker box to the scheduler to create and modify the schedule,
- commit to the schedule
- then, there should be a "carry out the plan option"