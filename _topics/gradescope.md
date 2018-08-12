---
topic: "Gradescope Info for TAs/Readers"
desc: "Scanning Homeworks to Gradescope, and grading"
---

The process:

1. Go through and make sure all paper is facing the right way.  Set aside any stapled, paper clipped, or other "odd" papers.
2. Scan papers to a PDF file.
3. Go to <https://gradescope.com> and pull up the course.  Go to the page where you can add an assignment.
4. You will need a PDF of the assignment.  The course page is here: <https://ucsb-cs56-f17.github.io>.  Find the homework, and "print to PDF".
5. Upload the PDF.  Name the assignment exactly what it is named on the course page (e.g. h00, h01, ic02, etc.)

# Notes on giving effective feedback

Be aware that when you write out the rubric items, <b>students see these rubric items.</b>

It is possible to hide the rubric items that are not applied to a student's submission, but Conrad prefers that all students see all of them.  The reason is that the main purpose of the homework is not "summative assessment" (assigning a grade), but rather "formative assessment"--helping students track their own learning, and improve their learning.

That's educational buzzword speak to mean: we need to give rich feedback to the students on what they know, and what they don't know.  We need to help them understand what kinds of answers we were looking for, and why some of the common incorrect answers are wrong.   The rubric on Gradescope is one place we can communicate that.

Another place is via a "summary" that you might post to Piazza after all the grading is done.  Consider making a Google Drive document, or even just a text file in an editor as you go through grading, and then when all is finished, post that to Piazza to help the students study.

# Rubrics

When I release a graded hwk or exam to the students, you can be sure that they will be like "tough reviewers" of a paper---scrutinizing what you wrote on the rubric, and what they wrote in their answer, and comparing answers with their friends like little lawyers trying to make a case.     

Our best opportunity to avoid problems is before we release the assignment.    I want to be sure that we have a clear rubric so that any grade disputes can be settled by simply "appealing to rubric".

Here

* +10: Full credit.  Answers may vary, but here is a sample answer. 

   The compiler translates Java source code to Bytecodes.  The Bytecodes are like an abstract instruction set for
   an imaginary computer.  The Java Virtual Machine is a program that simulates the execution of this imaginary computer, and
   executes Java bytecodes as if they were machine instructions.
   
   Note that the full credit answer clearly addresses three points: 
   (A) Java compiler translates source to bytecode (B) Bytecode is an abstract
   instruction set and (C) The JVM is a virtual machine that executes bytecodes.  
   
* +9:   This answer made the points A and B, but wasn't clear about C.
* +8:  This answer made points A and C, but wasn't clear about B
* +5:  This answer made only one of the three points A, B or C.  For full credit, you needed to make all three points.
* +2:  This answer contains some correct information, but does not clearly address any of points A, B or C.

That kind of rubric makes it possible for me, as an instructor, as well as for the student, to look at the answer they wrote, the grade you assigned, and the rubric, and see that "given the rubric, there is only one grade that could have been assigned."

That is, the rubric needs to be more or less a kind of "algorithm" that tends to produce the same results.  There may be some little bit of judgement call, but at least 80% of the time, two graders looking at the same problem and the same rubric would come up with the same answer.
