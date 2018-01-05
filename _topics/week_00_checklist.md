---
topic: "Week 0 Checklist"
desc: "Tasks for Mentors, TAs, Instructors before quarter starts"
---

# Instructor Setup for This Site

1. Change the value of `current-quarter-github-org` in [`_config.yml` of this repo](https://github.com/ucsb-cs56-pconrad-mentors/ucsb-cs56-pconrad-mentors.github.io/blob/master/_config.yml).  For example:

```
current_qtr_github_org: ucsb-cs56-w18
```

The current value of that setting is: <tt>{{ site.current_qtr_github_org }}</tt>

# Instructor Github Org Setup

1. Make sure that the Default repository permission is "None" on the <tt>{{ site.current_qtr_github_org}}</tt> settings. Those can be accessed at <https://github.com/organizations/{{site.current_qtr_github_org}}/settings/member_privileges>. 
This is SUPER important.  Otherwise, all students have read permission to even private repos.  That is clearly not desirable!

#  Instructor Other

1.  Mentors fill out the signup form for CS192/196 credit.   Get Instructor's signature.  Turn in to CS Dept. staff undergrad advisor,
     get add code, and sign up for course.   Note that signup is NOT automatic after you fill out form.  You MUST take the add code
     and actually sign up.
     
2.  Instructor provides form for Mentors to fill out with: fname,lname,umail,github_id,google_drive_email,csil_username,cell_phone

3.  Instructor creates slack channel, cs56-qxx-team (qxx is F16, F17, W17, etc.).   Adds all mentors to slack channel.

4.   Instructor adds mentors as owners on github orgs


# Accounts that TAs and Mentors Need

| Account Type |  TA?   | Mentor?   |
|--------------|--------|-----------|
| Github orgs (see below) |  Y     |    Y      |
| Gradescope   |   Y     |   No, for now |
| submit.cs    |   Y     |  No, for now |
| Piazza       |   Y     |   Y    |
| Google Drive Folder | Y    |  Y    |



# Github orgs that mentors should be added to:

* <https://github.com/orgs/ucsb-cs56-pconrad-mentors/people>
* <https://github.com/orgs/ucsb-cs56-pconrad/people> 
* <https://github.com/orgs/UCSB-CS56-Projects/people> 
* <https://github.com/orgs/ucsb-cs56-f16/people> (substituting current qtr in place of f16)



