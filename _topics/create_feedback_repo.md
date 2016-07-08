---
topic: "Creating feedback repos"
desc: "A private repo that students can read, but not edit"
---

One of the ways that mentors can give feedback (NOT GRADES) to students in CS56 is via the use of private feedback repos.

The private repos are read/write for course staff (organization owners, including instructors, TAs, and mentors), but read only
for the students.

Eventually, we will have an automated way to create these feedback repos, but for now it is still a manual process.  Fortunately,
as long as the mentor / mentee ratio remains fairly small (each mentor having between 3 and 10 pairs), the creation process does not
take very long.

The naming convention is as follows.  Put the githubids in alphabetical order.

* FEEDBACK_githubid1_githubid2 for pairs 
* FEEDBACK_githubid1_githubid2_githubid3 for trios
* FEEDBACK_githubid for individuals

To create these repos:

* Go to the web page of the organization for the course
    * For example, for M16, it is <https://github.com/UCSB-CS56-M16>
* Consult the list of legacy code project assignments
    * For example, for M16 it is: [lab/lab02/repo_list.md](https://UCSB-CS56-M16.github.io/lab/lab02/repo_list/)
* For each pair,trio,individual: create a private repo with this name.
    * Initialize it with a README.md.  
    * You don't need a .gitignore or a LICENSE file.
* After creating each repo, add each of the individuals with READ ONLY access to the repo.  You do this by adding them as collaborators.


