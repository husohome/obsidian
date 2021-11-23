# productivity bookkeeper


1. a tool to implement this [[High-School-Book-Keeperapproach to productivity]] idea. The design is meant to be opinionated.

#java #coding #productivity #to-do #productivity-book-keeper #project

# To-do
- [ ] design the program

# Structure
1. plan: spring-boot + Vue.js
2. just use decoupled
	1. represent everything as database tables
	2. call api s to update the database with, that's it
	3. let frontend visualize the data

# Essential features
1. design "courses" and set credits (weekly hours)
	1. maybe a profile?
2. daily to-do list/ scheduler or something like that which is linked to courses and credits
	1. and the ability to schedule recurring events?
3. some space to comment on the progress and give reflections
4. track how many credits have been spent for the week
5. basic and useful statistics
6. (temporarily no need for the User model, may include User in the future)

# how the users would interact with this app
1. [[Creating a course plan]]
2. [[Scheduling how to execute the course plan (weekly schedule)]]
3. [[Daily scheduler]]
4. [[To-do (basic execution unit)]]
5. others recorded in this note.


# Classes
1. [[Classes in productivity bookkeeper]]

# How to Show Progress?
coursePlan




# View-based overview

## Manual and Documentation
1. should be full of pictures
2. gives examples of how to use this web app
3. state something like: this is an opinionated app based on the plan laid out here
	1. based on [[High-School-Book-Keeperapproach to productivity]]
	2. and promodoro method!

## Workspace View
1. collapsible listings of course plans
	1. before expanded, show
	 	 - "name of the course plan"
	 	 - progress (needs to integrate with progress; need to think about how this is )
1. box2
	1. all unique courses ever designed (drag and drop)
	2. maybe some foreign key of when it is used? (search optimization?)

## Scheduler View(s)
1. course pane
	1. the course hours you need to plan (linked to course plan or other schedulers)
	2. drag and drop courses to the schedule pane
2. scheduler pane

## To-Do view
1. to-do items (clickable), once it's done, it feeds back to the progress

	
# Problems/ Questions/ Issues
1. is it necessary to see Course and the courses in the CoursePlan separately?
2. is it possible to expand the models to include sub-modules after we assume the basic unit is the course?
3. scheduler views feel very similar, so they could be children-and-parents
4. auto-save progress/ temporary ui components?
6. 

# Settings
1. appearance?
	- at least a light theme and a dark theme

