---
topic: "Week 0 Instructor Checklist"
desc: "Tasks for Instructor before quarter starts"
---

# Instructor Setup Steps

1. *Set value of `current-quarter-github-org` in `_config.yml`

   Change the value of `current-quarter-github-org` 
   in 
   [`_config.yml` of this repo](https://github.com/ucsb-cs56-pconrad-mentors/ucsb-cs56-pconrad-mentors.github.io/blob/master/_config.yml).  
   For example:

   ```
   current_qtr_github_org: ucsb-cs56-w18
   ```

   The current value of that setting is: <tt>{{ site.current_qtr_github_org }}</tt>

1. *Default Repository Permission Should be None on github org*.   

   Make 
   sure that the Default repository permission is "None" 
   on the <tt>{{ site.current_qtr_github_org}}</tt> settings. 
   Those can be accessed at <https://github.com/organizations/{{site.current_qtr_github_org}}/settings/member_privileges>. 
   This is SUPER important.  Otherwise, all students have read permission to even private repos.  That is clearly not desirable!

1. Create a form to collect information from instructional staff.    Examples of past forms include:
    * [CS56-F17-Mentor-Info](https://docs.google.com/forms/d/1NFRtNhKddOgGrIIWV16nLfrykSo_hDMwS5JfVNhxv78/edit)
    * [CS56-W18-Mentor-Info](https://docs.google.com/forms/d/1SZgLzL2vfY61D7653PEuerUNf7zjtJsXzE0GFlSacV4/edit)
    

1. Create a slack for instructional staff.  Naming convention is `ucsb-cs56-w18-team`
   Invite TAs, Readers, and Undergrad mentors.

1.  Mentors should be registered as paid mentors, or for CS190J credit. Verify that this is taken care of.
     
1.  Add instructional staff with access to various accounts as shown in table below:


   | Account Type |  TA?   | Mentor?   |
   |--------------|--------|-----------|
   | Github orgs (see below) |  Y     |    Y      |
   | Gradescope   |   Y     |   No, for now |
   | submit.cs    |   Y     |  No, for now |
   | Piazza       |   Y     |   Y    |
   | Google Drive Folder | Y    |  Y    |


   Github orgs
   
   * <https://github.com/orgs/ucsb-cs56-pconrad-mentors/people>
   * <https://github.com/orgs/ucsb-cs56-pconrad/people> 
   * <https://github.com/orgs/ucsb-cs56-projects/people> 
   * <https://github.com/orgs/{{site.current_qtr_github_org}}/people> 



