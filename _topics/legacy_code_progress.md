---
topic: "Legacy Code progress"
desc: "What mentors should be doing while students are assigned to work on legacy code"
---

This article describes what mentors should be doing during the time that students are assigned to work on legacy code, 
such as during these labs:

* [UCSB CS56 M16 lab04](http://ucsb-cs56-m16.github.io/lab/lab04/)
* [UCSB CS56 F16 lab05](http://ucsb-cs56-f16.github.io/lab/lab05/)


By the end of the lab meeting where lab04 is introduced, the following should be true:

* You've [created a feedback repo for each of your teams](/topics/creating_feedback_repos/)
* You've handled the [pull request from their first look at legacy code lab](/topics/pull_request_first_look_legacy_code/) and added feedback to their repos for it&mdash;at least as far as you can given their state of completion.
* You've communicated with each of your mentees about their labs for completion for lab04, and you've recorded some feedback on that in their feedback repo.

More on each of these items below.

# Creating Feedback Repos

See [created a feedback repo for each of your teams](/topics/creating_feedback_repos/).  Do this first.

# Check in with each pair (trio, individual)

The most important thing for you to do during lab is to *proactively* check in with *each pair* (or individual or trio) assigned to you
that should be there in lab.

The first thing to check is: "did they show up?"  If they did not, send them a message (I suggest via private message on Piazza, cc'd to "Instructors")
that asks about their welfare.    You can keep it friendly, and you can "assume", to help them save face, that they are not in lab for a good reason, i.e.
that they are sick, had a car accident, etc.   So, ask something like the following.  Put it in your own words, using whatever
way of communicating is natural for you.

>    I'm concerned because I didn't see you in lab.  
>    Is everything ok? I hope you are not sick, and that you were not in an accident, etc.
>    Please check in with me about your progress as soon as you can.  
>    As your mentor, I'm responsible (for my
>    own course grade) to help you succeed in the course as best I can.
>    Please let me know where you stand with (here, mention whatever work is due).

# Checking on their progress

The second thing is to check on their progress.  Students may have a tendency to be "behind", say working on lab03, when they should be finished with it by now and working on lab04.  Or they may not even have finished lab02.

In this case, encourage them to finish up lab03 (or lab02, or whatever), and try to get them to commit to some timeline for finishing.  Ask if they 
are "stuck" on anything specific.  

In general, encourage your mentees to be in touch with you, or post on Piazza, if they run into problems.
Remind them that they can post private messages to you on Piazza.  Remind them they can include, or not include, their instructors,
their pair partners, etc. on those messages.

# Handling pull request for first look at legacy code (e.g. [F16 lab03](http://ucsb-cs56-f16.github.io/lab/lab03/)).

This has been relocated to this page: [feedback_first_look_legacy_code]


# Handling pull requests for first round of legacy code work (e.g. [F16 lab05](http://ucsb-cs56-f16.github.io/lab/lab05/)).

For this lab, handling pull requests is a bit more involved.

You should do at least the following due diligence:

* Clone their repo (not the UCSB-CS56-Projects one, but their fork of it), yourself, and try compiling, running, etc.
* Note any problems you encounter.
* Check which issues the students claim to be closing with the pull request.  See if you are satisfied that the issue is resolved. IF NOT, THEN REOPEN THE ISSUE WITH FEEDBACK.  
* In your "public" feedback, i.e. the feedback in the issue itself, be VERY DIPLOMATIC and VERY FACE SAVING. Make only factual statements.   If there is anything too harsh or embarassing, put it in the PRIVATE feedback repo, and just make reference to that in the issue comments. For example: "Pull request 7 does not completely resolve issue 11, so I am reopening it. In particular, the bug when you click on the foobar button still seems to be present. See the private feedback repo for more details."  
* In the private feedback repo, you could say things like that are more critical: "We discussed structuring the code like x, but it appears you did not follow my advice. I wonder whether you may like to fix some of the indentation and remove some of the seemingly irrelevant comments that pertain to code that has already been removed."  Even there, try to practice diplomacy.
* If issues are closed successfully, and you think the points awarded are in order, then note this in the feedback repo under the lab04 section (even if the students did this as part of a pull request for lab02.)  In the feedback repo, put links to the issues and the pull requests.

If the pull request does in fact improve the code, and does not make anything worse, then *accept the pull request* and note that you did so in the feedback repo.  Delay accepting the pull request ONLY if/when there is some serious problem with the code the students have written.    

If you do NOT think you can accept the pull request, then the sooner you indicate this, and the specific concerns you have, the better.  The worst situation is to end up at the end of the course, on July 27,28, 29,30, for example, with three dozen unresolved pull requests across 15 repos.   Please don't let that happen!   Deal with them as soon as you can!

# How grading works

TAs: please set up proj1 and proj2 as assignments in Gauchospace worth 250 points, but with NO file submission, NO online text---unclick all of the boxes for students to submit things.   

* The students don't submit anything but pull requests that resolve issues. 
* The mentors are responsible for handling the pull requests, and putting information in the feedback repos.
* TAs are responsible for making a sweep through the feedback repos, and as they see information about closed issues, making an independent judgment about each case.  If you see that the issue is closed, and you are satisfied with the point value assigned, then do these two things:

1. NOTE that you have awarded points in the FEEDBACK repo.  
    * This note should have your initials (P.C., K.D., H.J. or R.J.), i.e initials of an instructor or a TA
    * The commit should also be done by the github id of an instructor or TA
    * It should indicate how many points were awarded.
    
2. In the feedback repo, near the bottom, add a section "Points awarded by instructors/TAs"
    * Here, just make a running tally of the points added into proj1, proj2, proj3, proj4.  
    * This section should answer the question: the 250 points in proj1, and the 100 points in proj2, where do they come from?
    * The answer should be found here as. (See example below).
    
3.  Record or update the current point total for proj1, proj2, proj3, or proj4 in Gauchospace.
    
```
# Points awarded by TA/Instructor

## proj1

* 200: all 200 points from issue #7
* 50: first 50 of 150 points for issue #8

Total: 250

## proj2

* 100: last 100 points of 150 for issue #8.

Total: 100

## proj3

no points awarded yet

## proj4

no points awarded yet

```
```


    
