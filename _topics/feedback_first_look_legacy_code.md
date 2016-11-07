---
topic: "Feedback: First-look-at-legacy-code-lab (F16 lab03)"
desc: "How mentors handle the pull requests for F16 lab03"
example_md_file: "F16_lab03.md"
---

# Handling pull request for first look at legacy code (e.g. F16 lab03)

These instructions pertain to:

* [M16 lab02](https://ucsb-cs56-m16.github.io/lab/lab02/)
* [F16 lab03](https://ucsb-cs56-f16.github.io/lab/lab03/)

So, "accepting" or "not accepting" the pull request for this lab is your responsibility.  You should have the authority (meaning the github.com permissions) to do so.  If you don't, ask the TA or instructor to adjust the settings (or even a fellow mentor that does have access.)   As a mentor, you should be an "owner" of the UCSB-CS56-Projects organization.

To decide whether to accept the pull request for the legacy code code review is usually easy.

If the only change is adding a <tt>{{page.example_md_file}}</tt> file, then just accept the pull request no matter what.

If they have also made changes that involve changes to code--i.e. fixing things that they might want to get points towards a future lab lab04, then see the page [Feedback on Legacy Code Progress](/topics/legacy_code_progress/) page for more instructions.


# After accepting the pull request

Immediately after accepting it, go into the [feedback repo](/topics/create_feedback_repo/) for that pair and add feedback under a heading for this lab in the README.md file.

The feedback you should add is this:  Check the items in lab instructions, for example:

* [F16 lab03](https://ucsb-cs56-f16.github.io/lab/lab03/)

For each one, did they do it or not?   

You should fill in a table such as this one (this is the format that John posted in the general channel on slack on Thu 10/27/2016):

```
| Item | +o?-  | Poss | Pts | Summary | Comments  
|------|-------|------|-----|-------------|-----------
| a    |       |  20  |     | A brief description of the project. | 
| b    |       |  20  |     | a set of user stories that describe the current software in its current state |
| c    |       |  20  |     | a brief assessment of whether the software runs. If it runs, briefly describe what it does   |
| d    |       |  20  |     | a set of user stories (at least 2) about features that COULD be added    |
| e    |       |  20  |     | An assessment of the current quality of the README.md. What information could be added?    |
| f    |       |  20  |     | An assessment of the current state of the build.xml file. |
| g    |       |  20  |     | An assessment of the current “issues”.    |
| h    |       |  20  |     | A list of additional issues that you may have added, if any  |
| i    |       |  100 |     | an assessment of the actual code   |
| j    |       |  40  |     | how is the test coverage?   |
```

Mentors: You are ONLY to fill in the `+o?-` column, NOT the Pts column.  Repeat: DO NOT FILL IN THE PTS Column.  That is for the TA, Reader or instructor to do.

You are not assigning a "grade", but you are making a check list and commenting on each item and drawing attention to things that are either particularly good, acceptable, or missing or problematic.  Think of it as making a checklist of  +, ok, -.  

Note that this is *not a grade*.  It is "feedback".  

True: the TAs might use it in deciding where to put their attention when assigning a grade, but they will make an indepdendent judgement before doing so.    This is a *very* important distinction to preserve, not just as a "notion", but in spirit and in truth.

You may also add some encouraging comment or hints about what the students should be doing as they move into the "complete the first 250 or 500 points of their assignment" phase (i.e. the lab where they have the first deadline for work on the legacy code project.)


