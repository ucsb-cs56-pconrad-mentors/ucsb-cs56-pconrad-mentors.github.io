---
topic: "Feedback: graphics lab part 1"
desc: "Mentor, TA and Instructor guidance on evaluating graphics lab part 1"
---


For the feedback repo for [lab06 from M16](https://ucsb-cs56-m16.github.io/lab/lab06/), follow the instructions here:

# HOW TO DEAL WITH PULL REQUESTS (as a moderator) for lab06

Step 1:

In the students's [individual FEEDBACK_githubid repo](), create a section called "lab06 feedback" 

In that section, copy paste the following text below (Sample Rubric as Github Flavored Markdown Table).

Step 2: Moderator fills in ONLY the +-o? column and the comments column.

THEN the moderator is ready to accept the pull request.  You can also comment on the pull request directly in the github.com UI, by commenting on lines of source code in the usual way.


# Sample Rubric as Github Flavored Markdown Table

Feedback goes into a PRIVATE repo on github.com under the UCSB-CS56-W16 organization, that is shared ONLY with that individual student.        

Normally we do that with scripts, but we might or might not end up doing that by hand this year if it ends up being easier--especially if we can divide up the work and have each of the moderators do that as they handle the feedback for each pull request.  It doesn't take long, and it only has to be done once per student per quarter.

Here's the raw stuff to copy/paste.   Each moderator should copy/paste this into the feedback, and then fill out ONLY the +o-? column, and the comments column.

to do the grading we need to change the line in the build.xml file that starts with   <property name="studentName" value="edtropiax"/>  to the real student csil username.

** or you can use >> export USER="csilUsername" from the command line to tell ant to access the proper package **

Step 3:  The TA or instructor fills in the numbers in the grade column, totals, and posts the grade to Gauchospace.

```
* + o - are indications from Moderator's review
 * o is **ok**, met expectations (no deductions),
 * - **below expectations** (deduction might be made by TA or instructor), 
 * + means **exceeds expectations** 
  * In rare cases, instructor or TA might award points to offset other deductions. No guarantee of this.
 * ? is a flag used by moderators to raise a **question** for the TA to investigate further
* Poss: Possible Points
* Pts: Points Awarded (only filled in by TA or Instructor, NOT by moderator)

| Item | +o?-  | Poss | Pts | Summary | Comments  
|------|-------|------|-----|-------------|-----------
| SG1  |       |  20  |     | SimpleGui1 text, color | 
| SN1  |       |  40  |     | Snowman has head   |
| C1   |       |  20  |     | correct package   |
| C2   |       |  20  |     | extend GeneralPathWrapper, implement Shape    |
| C3   |       |  50  |     | one class inherits from other    |
| C4   |       |  40  |     | constructor inits wrapper GP object |
| C5   |       |  40  |     | object looks reasonable    |
| C6   |       |  40  |     | coding style good  |
| GP   |       |  30  |     | followed instructions   |

```

Here's what it looks like when formated:

* + o - are indications from Moderator's review
 * o is **ok**, met expectations (no deductions),
 * - **below expectations** (deduction might be made by TA or instructor), 
 * + means **exceeds expectations** 
  * In rare cases, instructor or TA might award points to offset other deductions. No guarantee of this.
 * ? is a flag used by moderators to raise a **question** for the TA to investigate further
* Poss: Possible Points
* Pts: Points Awarded (only filled in by TA or Instructor, NOT by moderator)

| Item | +o?-  | Poss | Pts | Summary | Comments  
|------|-------|------|-----|-------------|-----------
| SG1  |       |  20  |     | SimpleGui1 text, color | 
| SN1  |       |  40  |     | Snowman has head   |
| C1   |       |  20  |     | correct package   |
| C2   |       |  20  |     | extend GeneralPathWrapper, implement Shape    |
| C3   |       |  50  |     | one class inherits from other    |
| C4   |       |  40  |     | constructor inits wrapper GP object |
| C5   |       |  40  |     | object looks reasonable    |
| C6   |       |  40  |     | coding style good  |
| GP   |       |  30  |     | followed instructions   |

## Lab05 pull request

Step 1: Determine the github.com ids for the two students (only one did the pull request, but the other is part of the pair.  If the two are not available on the pull request, you can look at the Spreadsheet with the name "snapshot" on the Google Drive.)

Step 2: Under the UCSB-CS56-W16 organization create a PRIVATE repo called cs56_w16_feedback_githubid1_githubid2.  For example for cgaucho and jole, create: cs56_w16_feedback_cgaucho_jole

It should have a README.md, but it need not have a gitignore or a license.

Step 3: Give students at least read access to their pair feedback repo.

Add the students as a collaborators on the student's feedback repo and add them OR create a team called e.g. Pair_github1_github2, e.g. Pair_cgaucho_jole with read access, and give them read access that way.  The mentor team can decide which is easier.

Step 4:  In the repo, create a file called lab05_feedback.md (which can be done directly in the github.com web interface by clicking the'+' after the repo name/--you do NOT need to clone, etc. unless you really really want to.)

In that file, copy paste the following text below (See Lab05 Rubric that Omeed created below).

Step 5: Moderator fills in ONLY the +-o? column and the comments column.

THEN the moderator is ready to accept the pull request. (If you already accepted it, no problem.) You can also comment on the pull request directly in the github.com UI, by commenting on lines of source code in the usual way.    Please then let the TA/Reader for your team know by his/her preferred method (email, a spreadsheet, whatever) that the lab05 is ready to be graded.


TODO: Adapt rubric below to M16 lab06


## Lab05 Rubric
```
CS56 W16 Lab05 Rubric

* + o - are indications from Moderator's review
 * o is **ok**, met expectations (no deductions),
 * - **below expectations** (deduction might be made by TA or instructor), 
 * + means **exceeds expectations** 
  * In rare cases, instructor or TA might award points to offset other deductions. No guarantee of this.
 * ? is a flag used by moderators to raise a **question** for the TA to investigate further
* Poss: Possible Points
* Pts: Points Awarded (only filled in by TA or Instructor, NOT by moderator)

| Item | +o?-  | Poss | Pts | Summary | Comments  
|------|-------|------|-----|-------------|-----------
| a    |       |  20  |     | brief description of project         | 
| b    |       | 20   |     | User stories that describe what current software can do  |
| c    |       |  20  |     | does software run?        |  
| d    |       |  20  |     | at least 2 user stories |
| e    |       |  20  |     | current state of the README          |
| f    |       |  20  |     | current state of the build.xml file  |
| g    |       |  20  |     | assessment of the current issues      |
| h    |       |  20  |     | additional issues            |  
| i    |       | 100  |     | assessment of the code itself        |
| j    |       |  40  |     | how is the test coverage?        |
```

CS56 W16 Lab05 Rubric

* + o - are indications from Moderator's review
 * o is **ok**, met expectations (no deductions),
 * - **below expectations** (deduction might be made by TA or instructor), 
 * + means **exceeds expectations** 
  * In rare cases, instructor or TA might award points to offset other deductions. No guarantee of this.
 * ? is a flag used by moderators to raise a **question** for the TA to investigate further
* Poss: Possible Points
* Pts: Points Awarded (only filled in by TA or Instructor, NOT by moderator)

| Item | +o?-  | Poss | Pts | Summary | Comments  
|------|-------|------|-----|-------------|-----------
| a    |       |  20  |     | brief description of project         | 
| b    |       | 20   |     | User stories that describe what current software can do  |
| c    |       |  20  |     | does software run?        |  
| d    |       |  20  |     | at least 2 user stories |
| e    |       |  20  |     | current state of the README          |
| f    |       |  20  |     | current state of the build.xml file  |
| g    |       |  20  |     | assessment of the current issues      |
| h    |       |  20  |     | additional issues            |  
| i    |       | 100  |     | assessment of the code itself        |
| j    |       |  40  |     | how is the test coverage?        |


## Lab06 Rubric: don't forget to git checkout animbranch before grading!

```

* + o - are indications from Moderator's review
 * o is **ok**, met expectations (no deductions),
 * - **below expectations** (deduction might be made by TA or instructor), 
 * + means **exceeds expectations** 
  * In rare cases, instructor or TA might award points to offset other deductions. No guarantee of this.
 * ? is a flag used by moderators to raise a **question** for the TA to investigate further
* Poss: Possible Points
* Pts: Points Awarded (only filled in by TA or Instructor, NOT by moderator)


| Item | +o?-  | Poss | Pts | Summary | Comments  
|------|-------|------|-----|-------------|-----------
| SG1  |       |  50  |     | in correct branch | 
| SN1  |       |  50  |     | animation works   |
| C1   |       |  50  |     | coding style      |
| GP   |       |  0-50 Extra Credit  |     | animation is AWESOME!   |

```
