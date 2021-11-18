
# Classes in Productivity Bookkeeper
#java #coding #productivity #to-do #productivity-book-keeper #project 


## Workspace
CoursePlans


## CoursePlan
1. collection of CourseLets
	
## CourseLet
1. fk: CoursePlan
1. fk: **Course**
	1. name
	2. description
	3. completion_action
		1. **CompletionAction**.QUAL
		2. CompletionAction.QUANT
		3. CompletionAction.BOTH
		4. CompletionAction.NEITHER
2. required credits: int
3. completed credits: dynamically generated from
	1. tasks
		1. check completion status
4. 

##  Task/ ToDO
completion status


# Progress
1. checks progress for you. Every time we need to see the progress of something, we generate it using Progress.getProgress(pass in the object here);
2. the class calls Progress.getProgress(Object o)
3. based on its class, checks all the subunits' completion?
4. 

# Method: Complete()
1. based on completion action and the class of the object
2. 

# Reflections