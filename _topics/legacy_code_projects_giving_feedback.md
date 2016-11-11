---
topic: "Legacy Code Projects: Giving Feedback"
desc: "Mentor, TA and Instructor guidance on evaluating legacy code work"
first_legacy_lab: "lab05"
pre_legacy_lab: "lab03"
TA_reader_instructor_initials: "N.B., M.Z., J.C., or P.C."
---

# Outline of the process

Here is an outline of the roles and responsibilities for grading of legacy code work.

* The <b>students</b> will submit their work by making pull requests that resolve issues.  
    * This is the one and only way to submit work for the legacy code labs.
* The <b>mentors</b> are responsible for handling the pull requests, and putting information in the feedback repos.
* The <b>TAs and Readers</b>, as a team, under the supervision of the <b>instructor</b> are responsible for grading. 

# Mentors: Feedback on Pull Requests and Closed Issues

Once you have [created a feedback repo](/topics/create_feedback_repo/) for each individual, pair, or team working on a legacy code project, you'll want to
put something in that repo.   The guidelines below explain what to do.

# Mentors: Before Writing your Feedback

You should do at least the following due diligence:

* Clone their repo (not the UCSB-CS56-Projects one, but their fork of it), yourself, and try compiling, running, etc.
* Note any problems you encounter.
* Check which issues the students claim to be closing with the pull request.  See if you are satisfied that the issue is resolved. IF NOT, THEN REOPEN THE ISSUE WITH FEEDBACK.  
* In your "public" feedback, i.e. the feedback in the issue itself, be VERY DIPLOMATIC and VERY FACE SAVING. Make only factual statements.   If there is anything too harsh or embarassing, put it in the PRIVATE feedback repo, and just make reference to that in the issue comments. For example: "Pull request 7 does not completely resolve issue 11, so I am reopening it. In particular, the bug when you click on the foobar button still seems to be present. See the private feedback repo for more details."  
* In the private feedback repo, you could say things like that are more critical: "We discussed structuring the code like x, but it appears you did not follow my advice. I wonder whether you may like to fix some of the indentation and remove some of the seemingly irrelevant comments that pertain to code that has already been removed."  Even there, try to practice diplomacy.

# Mentors: Writing Feedback (but NOT grading)

The first thing to do is to put in a heading appropriate to the "round" of work that the students did.  
List it as "Mentor evaluation for..." with your name in parens.

For example:

<tt># Mentor evaluation for {{page.first_legacy_lab}}: first round of legacy code work  (Chris Helpfulperson) </tt>

Then, under that heading, list the issues that the students worked on.  It is helpful if you can:

* provide a link to the pull request.
* specify the issue number and title
* make that a clickable link to the issue
* write down the number of points that the issues was estimated for, along with any request from the
  students for additional points, where applicable.
  
Example:

```

Pull request: https://github.com/UCSB-CS56-Projects/cs56-games-hopscotch/pull/12

* [Issue: #7](https://github.com/UCSB-CS56-Projects/cs56-games-hopscotch/issues/7) Change the menu 

Original Estimate: 250.  Student Requesting 300 in comment.


* [Issue: #97 Update JUnit tests](https://github.com/UCSB-CS56-Projects/cs56-games-hopscotch/issues/97)

Estimate: 200 


* [Issue #26: Change Help Menu to Make it Non-Editable](https://github.com/UCSB-CS56-Projects/cs56-games-hopscotch/issues/26) 

Estimate: 50
```

Then, under each issue, put some comments to help guide the TA/Instructor that will do the actual grading.  

* If there are any bugs that you find, see whether the bugs were there in the code BEFORE the students worked on it. If the 
   bug is a NEW bug, that's something you'll want to mention.
* Look at the "diff" provided in the pull request.  Look at the code.  Observe whether the code looks well written,
   naming, indentation, general code style, whether the OOP aspects are improving, or getting worse, whether test
   coverage is improving, or getting worse, etc.
* Then, write a few words of overall feedback that will provide helpful information to  the TA/Instructor
   as they decide whether to award the exact number of points, fewer points, or extra points.
* It is probably *not* appropriate to specifically *recommend* exact, fewer, or extra points.  That looks and smells like
    "grading", which you are NOT authorized to do.   However, pointing out factual information such as the following is
    entirely appropriate:
    
    * The menu looks better than it did before
    * The code is better structured (or: more fragmented)
    * The test coverage is improved (or: more classes were added, but without any test coverage)
    * etc.
* If issues are closed successfully, then note this in the feedback repo under the {{page.first_legacy_lab}} section (even if the students did this as part of a pull request for {{page.pre_legacy_lab}}.)

Those things all send a signal to the TA/Instructor of what to look for, but stop short of recommending a specific action.
If you have any questions on this, please consult your instructor.

If the pull request does in fact improve the code, and does not make anything worse, then *accept the pull request* and note that you did so in the feedback repo.  Delay accepting the pull request ONLY if/when there is some serious problem with the code the students have written.    

If you do NOT think you can accept the pull request, then the sooner you indicate this, and the specific concerns you have, the better.  The worst situation is to end up at the end of the course with three dozen unresolved pull requests across 15 repos.   Please don't let that happen!   Deal with them as soon as you can!
  


# TA/Instructors: Do the grading 

Here's how grading works for TA/Readers/Instructors:

* Periodically, making a sweep through the feedback repos.
* As you see information about closed issues, make an independent judgment about each case.  
* As a TA/Reader doing grading, if/when, you see that the issue is closed, and you are satisfied with the point value assigned, then do these two things:

1. NOTE that you have awarded points in the FEEDBACK repo.  
    * This note should have your initials ({{page.ta_reader_instructor_initials}}), i.e initials of an instructor or a TA
    * The commit should also be done by the github id of an instructor or TA
    * It should indicate how many points were awarded.
    
2. In the feedback repo, near the bottom, add a section "Points awarded by instructors/TAs"
    * Here, just make a running tally of the points added into proj1, proj2, proj3, proj4.  
    * This section should answer the question: the 250 points in proj1, and the 100 points in proj2, where do they come from?


