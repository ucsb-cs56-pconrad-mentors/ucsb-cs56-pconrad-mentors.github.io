---
topic: "Feedback: graphics lab part 1 (F16 lab04)"
desc: "Mentor, TA and Instructor guidance on evaluating graphics lab part 1"
lab_num: "F17 lab04"
---


These are instructios for the feedback repo for:

* [lab04 from F17](https://ucsb-cs56-f17.github.io/lab/lab04/)
* [lab06 from M16](https://ucsb-cs56-m16.github.io/lab/lab06/)
* [lab04 from F16](https://ucsb-cs56-f16.github.io/lab/lab04/)


# HOW TO DEAL WITH PULL REQUESTS (as a moderator) for this lab

Step 1:

In the students's [individual FEEDBACK_githubid repo](/topics/create_feedback_repo/), create a section called "{{page.lab_num}} feedback"

In that section, copy/paste the following text below (Sample Rubric as Github Flavored Markdown Table).

Step 2: Moderator fills in ONLY the `+-o?` column and the comments column.

THEN the moderator is ready to accept the pull request.  You can also comment on the pull request directly in the github.com UI, by commenting on lines of source code in the usual way.

# Sample Rubric as Github Flavored Markdown Table

Feedback goes into a PRIVATE repo on github.com under the appropriate github organization for the course, that is shared ONLY with that individual student.    See: [Creating Feedback Repos](/topics/create_feedback_repo/)

Normally we do that with scripts, but we might or might not end up doing that by hand this year if it ends up being easier--especially if we can divide up the work and have each of the moderators do that as they handle the feedback for each pull request.  It doesn't take long, and it only has to be done once per student per quarter.

Here's the raw stuff to copy/paste.   Each moderator should copy/paste this into the feedback, and then fill out ONLY the `+o-?` column, and the comments column.

to do the grading we need to change the line in the build.xml file that starts with   <property name="studentName" value="edtropiax"/>  to the real student csil username.

** or you can use `export USER="csilUsername"` from the command line to tell ant to access the proper package **

Step 3: The Mentor marks column in Google Spreadsheet

In the Google spreadsheet where this is being tracked put an X in the column called "Lab04 Feedback Ready" 

* for F17 that sheet is this one: <http://bit.ly/cs56-f17-repo-sheet>

Step 4:  The TA (or instructor) fills in the numbers in the grade column, totals, and posts the grade to Gauchospace.

(For F17, Jonathan, Kevin B and Yun should divide up this duty among the three mentor teams.)

```
* \+ o - are indications from Moderator's review
  * o is **ok**, met expectations (no deductions),
  * \- **below expectations** (deduction might be made by TA or instructor), 
  * \+ means **exceeds expectations** 
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

* \+ o - are indications from Moderator's review
  * o is **ok**, met expectations (no deductions),
  * \- **below expectations** (deduction might be made by TA or instructor), 
  * \+ means **exceeds expectations** 
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

