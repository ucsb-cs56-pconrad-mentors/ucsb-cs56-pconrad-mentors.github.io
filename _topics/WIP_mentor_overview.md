---
topic: "WIP Mentor Overview"
desc: "Raw notes from J.C.--needs a reformat"
---

These are some raw notes from a document by Jenna Cryan.   As time permits, these could be crafted into a more coherent guide for CS56 mentors.


```
Team Leadership for Advanced Applications Programming
Expectations
As a team leader, there are certain expectations of conduct for this course. The main goals are to gain meaningful insight into working as a manager / scrum master while helping students learn about how to work on a project development team. It’s a learning environment for everyone involved, and at any point feel free to discuss anything with the other mentors, the mentor leader ( if there is one ), the TA(s), and especially with the professor. 
On a base level, mentors are there to lead their student teams and resolve questions and conflicts. Unlike TAs, readers, and professors, mentors do not evaluate the performance of the students in a quantifiable way. Evaluations of student work take place in the form of code reviews when the mentors have the opportunity to provide meaningful feedback on their code. 
Mentors are responsible for reviewing labs beginning around the fourth week of the quarter. The main bulk of code review comes from the legacy code projects, which the mentors and student teams should be in close contact regarding its progress throughout the quarter.
Moderators / Mentors
Leadership
Project manager / scrum master work duties
Plan sprints
Discuss with team their expectations for the quarter
Check in with team frequently
Ensure plans are being followed and work with team to ensure they have all that they need ready to complete the work that session
Code reviews
Code reviews offer the students a chance to improve their coding practices and mentors a chance to practice analyzing code for performance and best practices for industry. As a team leader or project manager in the real world, a significant goal is to generate an efficient, working piece of code. 
Although the student may have created something that works, it may not be well implemented and now is the opportunity to inform the student of ways to improve upon their code. Separate from their grade in the course, this is a time to show them how their code would be evaluated in the real world, based on a given project specification (not a grading rubric). This means that even if they have working code that satisfies the lab requirements, there may still be room for improvement that they were unaware of.
Any evaluations of student work may be used by the TAs or reader to gain insight into the code for future grading, but the evaluation should be based on the purpose of the code, not the grading rubric.
Labs
Lab preparation
Look over labs material, be prepared to answer questions
Do the lab if unfamiliar with concepts due to not remembering material or have not done it before
Lab time
Arrive a little early if possible
Sit at the head of a row on furthest end of the lab by the windows
If you aren’t leading a row of students during a lab session, find a free seat near the front or back
Oversee team members throughout lab session
Check in with students first
Make sure they know what they need to be doing and any deliverables for the week
Students are given until the following week to complete a lab. This gives them an opportunity to ask any last minute questions about the previous week’s lab, but it should be mostly completed before the following lab session so they have ample time to ask any necessary questions for the next lab. 
Legacy Code Projects
Curation of previous repositories
Look through projects in organization
https://github.com/UCSB-CS56-Projects
Update basic information from previous year
Copy any descriptions from the previous mentors and save it in the README 
Look through previous legacy work and merge any pull requests that look like they contribute to the project going forward
Make sure to run the code and make note of any incomplete or non-working features. These can be used as issues for students to work on, or it may be a sign that the code should not be merged but rather scraped
Most often, the code can be used going forward. The only time previous legacy code is rejected is if it really does not work well with future plans or severely broke the project in some way
Decide if repository should be assigned or not
If yes, fill in any new issues that sound interesting and mark it ready in the project description at the top of the repository (ie W16 - ready)
If no, then clean up anything from previous year and mark repository as not ready (ie W16 - not ready)
Generation of new repositories
Transition from Java Swing apps to Java web apps
Many of the current projects are from many years ago and consist of simple games with oldschool graphics that are not very interesting anymore
With the introduction of the Heroku lab, students can take any existing project and translate it into a Java web application.
Although there is no corresponding introductory lab, if any students have Android application programming experience, they can take any existing project and translate it into an Android application. They cannot, however, create an iOS application because the course is designed to teach object oriented programming in Java.
Additionally, new apps can be started for the students to work on.
To continue with the legacy code theme, and due to the complexities of web / Android application frameworks, the students  the mentors should start the project repository 
Point estimates
Points are estimated at 100 points is roughly 2 hours of work
Not a hard line in any way. Working on a bug for 2 hours, while still a good learning experience, wouldn't count the same as 2 hours of coding that perhaps created a menu screen, for example
Point estimates are subjective by nature, but are designed to be a guideline for amount work completed and to set a reasonable goal for
Code Reviews
As the team leaders, mentors know the most about the progress of their teams’ projects from start to finish and as such mentor feedback is very important
Any lab reviewed by a mentor will involve several steps:
Detailed instructions can be found at: https://github.com/UCSB-CS56-W16/W16-lab04/wiki
First, if the individual or team does not yet have a feedback repository on the current CS56 organization* then create one for them
*not the CS56 organization with all the project repositories, but for the current quarter
Create a team for the student/pair/group and add them to the repository with read only access to they may view but not modify your code reviews
Then, create a feedback markdown file for the current code to be reviewed 
i.e. lab04_feedback.md
The rubric that goes in the code review feedback readme is based off of the grading rubric just as a way to ensure they completed everything required. Mentor feedback should check that these requirements are fulfilled, but more importantly look through the code to give meaningful feedback in the comment section pertaining to coding style, efficiency, etc as you see fit.
Weekly Breakdown
Week 1
Meet with professor, TAs, other mentors to get to know everyone and discuss expectations for the quarter
Meet with students during lab, they may or may not be the same students on your team for the rest of the quarter
Week 2
Get to know your team members
Find out if any of them are interested in web or Android application programming, they may be better suited for another mentor with similar interests and programming experience who could provide more meaningful code reviews
Work out pairs / individuals
Some labs will be done in pairs, and some are to be done individually. Often, it’s easiest if pairs can be worked out early on in the quarter and that you know who is working by themselves and who is not. 
Although they are all responsible for the same work whether working individually or in a group, those working as individuals may need a little extra guidance to ensure they sufficiently plan out their work load, especially as it pertains to the legacy code project
Week 3
Help students work on Java programming skills
Labs such as the polynomial and animation labs should be mostly straightforward and help prepare them for working with the legacy code projects
Most questions end up relating to issues with Javadocs, so be sure to be familiar with how to deploy / debug those
Week 4
Assign projects
For simplicity, students are first arbitrarily assigned a project to do an initial lookover. They will get the opportunity the following week to switch it if they would like (for instance, if they would like to work on Android or web apps)
Week 5
Reassign projects if necessary
Some students may really want to switch from the project they were initially assigned, and now is their chance to voice that. If enough students want to switch or if there are extra repos to offer them as an alternative, they may be allowed to change
Furthermore, any students who wish to work on a Android or web application may speak up now and try to work on one of those repos
Meet with team members to go over plans for first sprint
Now the teams should have their projects and be able to begin planning that they would like to accomplish this quarter
Then, you should work together to figure out a plan for their first 2 week sprint
Week 6
Check in with progress of legacy code projects
Possibly rework goals that have been too complex for that team or add complexities to goals that were completed with ease
Make sure students know that just because something was estimated at a point value doesn’t mean they will necessarily get that many points
For instance, if they were able to generate a simple GUI for an application that took maybe an hour, they would not receive the same points as someone who dedicates more time into creating something more complex
Try to encourage students to have a form of working code by the end of the sprint, so they are ready to begin a new sprint for different issues
Week 7
Meet with students to go over first sprint
Code should be in a running state and ready for the next sprint going forward
Discuss challenges, revisions to project goal 
Discuss plans for next sprint
Should be a similar amount of work as the first sprint, and should result in a working final product that could be demoed at end of quarter
Week 8
Check in with progress of legacy code projects
Go over code reviews of last sprint with students
Again, rework any current issues
Main focus is having a solid working project that satisfies as many of the project specification goals as possible
Week 9
Check in with team members, demo projects
Ensure your expectations align with their expectations for total work completed
Go over code reviews for first sprint, if haven’t already to show them the current state of the project from your point of view
Week 10
Meet with student team members to go over final code review, if possible
Many projects may not be completed in time to review it with them in person, but a live demo should give mentors an opportunity to generally discuss if they met expectations
Discuss possible issues to add to repository for future generations of students
Working with TAs / reader
Work delegation
Mentors work mostly with the students themselves. However, at the start of the quarter, mentors should meet with the professor, TAs, and reader (if applicable) to discuss expectations for delegating work.
As the students finish their labs, it is important that the mentors begin reviewing them so as to provide speedy feedback and they have opportunity for improvement going forward
TAs and reader will always be in charge of actually grading, but they will wait for code review feedback from mentors as it signals the students are done and it is useful when reviewing their work. As such, it is important to maintain an open line of communication among all mentors, the TAs, reader, and at times also the professor in terms of exactly what has been done and what is left to be completed. Most conveniently, this can be handled through shared spreadsheets set up by a TA or mentor (or mentor leader if applicable) at the start of the quarter so everyone is on the same page, literally. Additionally, while mentors know what they are responsible for (their own teams work) the TAs do not have their work as easily delegated. The spreadsheet will also allow TAs or reader to ‘claim’ an assignment to grade to prevent overlap.
```
