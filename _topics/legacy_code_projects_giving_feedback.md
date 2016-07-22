---
topic: "Legacy Code Projects: Giving Feedback"
desc: "Mentor, TA and Instructor guidance on evaluating legacy code work"
---

Once you have [created a feedback repo] for each individual, pair, or team working on a legacy code project, you'll want to
put something in that repo.   The guidelines below explain what to do.

# Mentors: Do a review (but NOT grading)

The first thing to do is to put in a heading appropriate to the "round" of work that the students did.  
List it as "Mentor evaluation for..." with your name in parens.

For example:

```
# Mentor evaluation for lab04: first round of legacy code work  (Chris Helpfulperson)
```

Then, under that heading, list the issues that the students worked on.  It is helpful if you can:

* provide a link to the pull request.
* specify the issue number and title
* make that a clickable link to the issue
* write down the number of points that the issues was estimated for, along with any request from the
  students for additional points, where applicable.
  
Example:

```

Pull request: https://github.com/UCSB-CS56-Projects/cs56-games-hopscotch/pull/12

* [Issue: #7](https://github.com/UCSB-CS56-Projects/cs56-games-hopscotch/issues/42) Change the menu 

Original Estimate: 250.  Student Requesting 300 in comment.


* [Issue: #11 Update JUnit tests](https://github.com/UCSB-CS56-Projects/cs56-games-hopscotch/issues/97)

Estimate: 200 


* [Issue #26: Change Help Menu to Make it Non-Editable](https://github.com/UCSB-CS56-Projects/cs56-games-hopscotch/issues/25) 

Estimate: 50
```

Then, under each issue, put some comments to help guide the TA/Instructor that will do the actual grading.  

* Actually clone the repo, and run the code.  See whether the code works.
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

Those things all send a signal to the TA/Instructor of what to look for, but stop short of recommending a specific action.
If you have any questions on this, please consult your instructor.
  

# TA/Instructors: Do the grading

Insert a new section with a heading such as this (with your name in parens).

```
# TA/Instructor Grading for lab04: first round of legacy code work  (P. H. Diddy )
```

Copy paste the list of issues, and then just indiciate the points awarded for each.   If the points are the standard amount that was 
requested, no further explanation is needed.  If you award fewer points, or extra points, provide a brief explanation.


