---
topic: "CS56 Mentor Overview"
desc: "An overview of the roles and responsibilities of CS56 mentors; a guide for mentors, TAs/Readers, and instructors"
---

# Mentors for CS56: An overview 

This document provides an overview of the roles and responsibilities of Mentors in CS56.

<div style="font-size:80%" markdown="1">
Acknowledgments: The original outline was authored by Jenna Cryan.   Additional edits have been made by Angela Yung, Alex Thielk and Phill Conrad.
</div>

# Expectations of Mentors

**Be a team leader:** On a base level, mentors are there to lead their student teams and resolve questions and conflicts. Mentors are responsible for reviewing the labs of the students they are mentoring. Make sure you read this: [Basic Guidelines for TA/Reader/Mentor](/topics/TA_Reader_Mentor_guidelines/)

**Review legacy code projects:** The bulk of code review comes from the legacy code projects, which mentors will prepare. Mentors and student teams should be in close contact regarding its progress throughout the quarter. [Mentor Roles during Legacy Code work](/topics/mentor_roles_during_legacy_code_work/)

**Provide meaningful feedback to mentees:** Unlike TAs, readers, and professors, mentors do not evaluate the performance of the students in a quantifiable way. Mentor evaluations of student work take place in the form of code reviews when the mentors have the opportunity to provide meaningful feedback on student code and habits. Maybe useful: [Steps for Creating Feedback Repos](/topics/create_feedback_repo/)
  
# Learning Goals for Mentors
   
The main learning goals for students undertaking the mentor role as a CMPSC192 project course are:
   
* To gain meaningful insight into working as a manager / scrum master while learning&mdash;and helping students learn&mdash;about how to work on a project development team. 
* To practice and develop leadership and professional communication skills in the dual contexts of professional software development and CS Education
* To gain additional knowledge and skill and depth in Java-based software development beyond what was learned when the mentor took CS56 or an equivalent course.   This includes:
    * Knowledge of the Java language itself    
    * Skill with various tools and techniques as applicable.   The exact list will depend on the legacy code
         projects the mentor interacts with, but will always include git/github and Ant.
    * Other tools and techniques may include Android Development, Java web applications, Maven, Gradle, etc.


It’s a learning environment for everyone involved, and at any point feel free to discuss anything with the other mentors, the mentor leader ( if there is one ), the TA(s), and especially with the professor. 

# Duties of Mentors

**Project manager / scrum master work duties:** _As team leaders, it is important mentors work closely with teams to ensure they have everyting they need to complete the work for the quarter and succeed_

  * Help Students plan sprints and follow through on those plans
  * Discuss with team their expectations and goals for the quarter   
  * Check in with team frequently 
   
**Code reviews:** _As the team leaders, mentors know the most about the progress of their teams’ projects from start to finish and as such mentor feedback is very important. Detailed instructions for lab reviewed can be found at:_ [Link](https://github.com/UCSB-CS56-W16/W16-lab04/wiki/)

  * Help your teams improve on their code based on how code is evaluated in the real world. 
  * Give in-depth reviews. Even if they have working code that satisfies the lab requirements, there may still be room for improvement that they were unaware of.
  * Give evaluations based on the purpose of the code and project specifications, not solely based on the grading rubric.
  * Facilitate good coding practices that can continue to be built on to develop into something better.  
  * Encourage the use of design paterns and other course material.
    
**Lab preparation:**

  * Look over labs material, be prepared to answer questions
  * Do the lab if unfamiliar with concepts due to not remembering material or have not done it before
    
**Lab time:**

  * Arrive a little early if possible
  * Sit at the head of a row on furthest end of the lab by the windows
  * If you aren’t leading a row of students during a lab session, find a free seat near the front or back and be available to help other teams
  * Oversee team members throughout lab session
     * Check in with students first. Make sure they know what they need to be doing and any deliverables for the week
     * Give students the opportunity to ask any last minute questions about the previous week’s lab. Students are given until the following week to complete a lab.
  * Encourage students not to fall behind. The previous lab should be mostly completed before they come to lab. 
      
**Curation of Legacy Code repositories:**
  
  * More detailed steps about [The Curation Process](/topics/curation_start_of_course/)
  * Look through projects in organization: [Link of Projects list](https://github.com/UCSB-CS56-Projects)
  * Update basic information from previous year
  * Copy any descriptions from the previous mentors and save it in the README 
  * Look through previous legacy work and merge any pull requests that look like they contribute to the project going forward
  * Make sure to run the code and make note of any incomplete or non-working features. These can be used as issues for students to work on, or it may be a sign that the code should not be merged but rather scraped.
  * Decide if repository should be assigned or not.  Most often, the code can be used going forward. The only time previous legacy code is rejected is if it really does not work well with future plans or is severely broken in some way
    * If yes, fill in any new issues that sound interesting and mark it ready in the project description at the top of the repository (ie W16 - ready)
    * If no, then clean up anything from previous year and mark repository as not ready (ie W16 - not ready)
  * Look for additional issues that can be created to improve the code, whether it is improving the implementation/code structure or enhancing a user experience
  * Estimate how much points an issue is worth and assign it to new issues created.

**Generation of new repositories:**

  * Transition from Java Swing apps to Java web apps
  * Many of the current projects are from many years ago and consist of simple games with oldschool graphics that are not very interesting anymore
  * With the introduction of the Heroku lab, students can take any existing project and translate it into a Java web application.
  * Although there is no corresponding introductory lab, if any students have Android application programming experience, they can take any existing project and translate it into an Android application. They cannot, however, create an iOS application because the course is designed to teach object oriented programming in Java.
  * New apps can be started for the students to work on.
  * To continue with the legacy code theme, and due to the complexities of web / Android application frameworks, the mentors should start the project repository.
    
**Point estimates:**

  * Points are estimated at 100 points is roughly 3 hours of work. It is not a hard line in any way. Working on a bug for 3 hours, while still a good learning experience, wouldn't count the same as 3 hours of coding that perhaps created a menu screen, for example.
  * Point estimates are designed to be a guideline for the amount of work completed and to set a reasonable goal for students.
  
## Weekly Breakdown

**Week 0**
  
  * [Week 0 checklist](/topics/week_00_checklist/)
  * Read the following two articles: 
    * [Basic Guidelines for TA/Reader/Mentor](/topics/TA_Reader_Mentor_guidelines/)
    * [Mentor Roles during Legacy Code work](/topics/mentor_roles_during_legacy_code_work/)

**Week 1**

  * Meet with professor, TAs, other mentors to get to know everyone and discuss expectations for the quarter
  * Meet with students during lab, they may or may not be the same students on your team for the rest of the quarter
  
**Week 2**

  * Get to know your team members
  * Find out if any of them are interested in web or Android application programming, they may be better suited for another mentor with similar interests and programming experience who could provide more meaningful code reviews
  * Work out pairs / individuals
    * Encourage them to pair program.
  * Some labs will be done in pairs, and some are to be done individually. Often, it’s easiest if pairs can be worked out early on in the quarter and that you know who is working by themselves and who is not. This allows them to get used to each other before working on legacy code.
  * Although they are all responsible for the same work whether working individually or in a group, those working as individuals may need a little extra guidance to ensure they sufficiently plan out their work load, especially as it pertains to the legacy code project

**Week 3**

  * Help students work on Java programming skills
  * Labs such as the polynomial and animation labs should be mostly straightforward and help prepare them for working with the legacy code projects
  * Most questions end up relating to issues with Javadocs, so be sure to be familiar with how to deploy / debug those

**Week 4**

  * Assign projects
  * For simplicity, students are first arbitrarily assigned a project to do an initial lookover. They will get the opportunity the following week to switch it if they would like (for instance, if they would like to work on Android or web apps)
  * During this week's lab, they are asked to write readme files about their thoughts of the projects and do pull requests. 
  * Mentors are going to create feedback repos for each group of students as well as for each individual student [Steps for Creating Feedback Repos](/topics/create_feedback_repo/)
  * Mentors will have to deal with pull requests of students' readme files about their feedbacks on the initial look of the project [Steps for Accepting Pull Requests (First look at Ledacy Code)](https://ucsb-cs56-pconrad-mentors.github.io/topics/feedback_first_look_legacy_code/)

**Week 5**

  * Reassign projects if necessary
  * Some students may really want to switch from the project they were initially assigned, and now is their chance to voice that. If enough students want to switch or if there are extra repos to offer them as an alternative, they may be allowed to change
  * Furthermore, any students who wish to work on a Android or web application may speak up now and try to work on one of those repos
  * Meet with team members to go over plans for first sprint
  * Now the teams should have their projects and be able to begin planning that they would like to accomplish this quarter
  * Then, you should work together to figure out a plan for their first 2 week sprint

**Week 6**

  * Check in with progress of legacy code projects
  * Possibly rework goals that have been too complex for that team or add complexities to goals that were completed with ease
  * Make sure students know that just because something was estimated at a point value doesn’t mean they will necessarily get that many points. For instance, if they were able to generate a simple GUI for an application that took maybe an hour, they would not receive the same points as someone who dedicates more time into creating something more complex
  * Try to encourage students to have a form of working code by the end of the sprint, so they are ready to begin a new sprint for different issues

**Week 7**

  * Meet with students to go over first sprint
  * Code should be in a running state and ready for the next sprint going forward
  * Discuss challenges, revisions to project goal 
  * Discuss plans for next sprint
  * Should be a similar amount of work as the first sprint, and should result in a working final product that could be demoed at end of quarter
  * Mentors need to go over students' progress on completing the first 500 points of their 1000 point goal by the end of the quarter. 
  * Mentors need to give feedbacks on students' half-completed legacy code project. [Steps for Giving Feedback on Legacy Code Projects](/topics/legacy_code_projects_giving_feedback/)
  * What to do when you get a pull request for the legacy code projects: [Deal with Legacy Code pull requests](/topics/legacy_code_pull_requests/)

**Week 8**

  * Check in with progress of legacy code projects
  * Go over code reviews of last sprint with students
  * Again, rework any current issues
  * Main focus is having a solid working project that satisfies as many of the project specification goals as possible

**Week 9**

  * Check in with team members, demo projects
  * Ensure your expectations align with their expectations for total work completed
  * Go over code reviews for first sprint, if haven’t already to show them the current state of the project from your point of view

**Week 10**

  * Meet with student team members to go over final code review, if possible
  * Many projects may not be completed in time to review it with them in person, but a live demo should give mentors an opportunity to generally discuss if they met expectations
  * Discuss possible issues to add to repository for future generations of students
  * Working with TAs / reader
  
**Final Week**

  * Mentors need to submit a End-of-Quarter Essay to the department [End-of-Quarter Essay](/topics/essay/)

# Work delegation

Mentors work mostly with the students themselves. However, at the start of the quarter, mentors should meet with the professor, TAs, and reader (if applicable) to discuss expectations for delegating work.

As the students finish their labs, it is important that the mentors begin reviewing them so as to provide speedy feedback giving them the opportunity to improve going forward and to catch any turn in issues before the grader.

TAs and reader will always be in charge of actually grading, but they will wait for code review feedback from mentors as it signals the students are done and it is useful when reviewing their work. As such, it is important to maintain an open line of communication among all mentors, the TAs, reader, and Professor at all times. Keep up with the professor in terms of exactly what has been done and what is left to be completed. Most conveniently, this can be handled through shared spreadsheets set up by a TA or mentor (or mentor leader if applicable) at the start of the quarter so everyone is on the same page, literally. 

Additionally, while mentors know what they are responsible for (their own teams' work) when there are multiple TAs/Graders, it isn't as clear which TA/Grader is responsible for grading which legacy code project.    The spreadsheet will also allow TAs and Readers a mechanism to ‘claim’ an assignment to grade to prevent overlap.

