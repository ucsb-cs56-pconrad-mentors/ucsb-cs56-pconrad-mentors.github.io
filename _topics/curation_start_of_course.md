---
topic: "Curation: start of course"
desc: "Getting legacy code repos ready for students to start work"
---

Older info: <https://foo.cs.ucsb.edu/56wiki/index.php/Curation>

Basic steps to doing initia

* Clone the repo.
* Review the README.md. 
    - If the README.md does not, at a minimum, have a brief description of what the project is
      supposed to be about, i.e. what the code does from a user standpoint and how to build and 
      run the project, add that yourself.
    - If the README.md is in pretty good shape, but there are still ways that the README.md could be improved, i.e with screenshots, developer documentation, and build/usage instructions, add the needed improvements as low point issues (e.g. 100 points).
* Ensure project can actually be built and run as intended (i.e. run the ant build.xml)
* Run `ant -p` and also inspect the `build.xml` file.
    * If there are targets without a `description` attribute, add fixing this as a low point issue
      (e.g. 50 to 100 points)
    * If there are parts of the build.xml that are obsolete (see below), add refactoring that
      as an issue.
    * Add as issues, any other obvious problems or refactorings in the build.xml
* Check the javadoc generation
    * Most of the current build.xml files, if they build javadoc at all, will
      publish it to a CSIL account.   
    * The javadoc files might be in the .gitignore
    * Instead, we should have them NOT put the javadoc in the .gitignore, and NOT copy it to
      a space outside the repo.   They should, instead, use the gh-pages workflow to publish
      their javadoc to a github pages URL.   Add this as an issue on every repo where
      the build.xml doesn't already do this (for M16, that will be every repo.  For quarters
      after M16, it will be a mix.)
* Check the javadoc itself
    * If there are places where the javadoc can be improved, note those as issues
* Check the existing list of issues
    * Familiarize yourself with each issue.
    * If the issue is a bug, try to reproduce the bug.  If the "steps to reproduce" are not
      clear in the issue, add some clarifications.  If you yourself cannot reproduce the bug,
      note that in a comment on the issue.     Don't delete the issue though; maybe someone else
      will be able to reproduce it.
    * If the issue is a feature request, does the issue provide enough detail that a student
      could get started on adding the feature?  If some additional detail is needed, provide it.
      Don't, however, do design "for" the students if they should be capable of doing that
      themselves.  Find a reasonable middle ground between "too vague" and "too specific".
* Try to find bugs.  If you find some that are not already listed as issues, add them.
* Review the user interface for potential improvements.  Consider adding those as issues.
* Look at test coverage (and noting which portions of the project have no test coverage)
    * Add issues to add additional JUnit tests anywhere that test coverage is not present.
    * If there are parts of the code base where junit testing is not feasible, but there are
      refactorings to make it more unit testable, add that as an issue.
* Identify portions of codebase that can be cleaned up and refactored and create corresponding issues
* Commenting on existing issues to ask clarifying questions, or point out any parts of the issues that are unclear.  Ask yourself---if I were assigned to work o this, would I know what to do and where to start? Or would I be confused and have questions? If its the latter, ask the questions in the comments.
* Identify uncommented portions of codebase, add normal and Javadoc comments to that portion of codebase, and/or change variable and method names to ones that make comments unnecessary/superfluous.
* Read build.xml and attempt to identify unecessary/obsolete/confusing portions of build script and make corresponding issues.
* Check package names
    * Some old projects may have package names that have specific quarters in the names.
    * Refactoring the package name to match the standard is a good issue to add if needed:
      `edu.ucsb.cs56.projects.x.y` where x is the high level topic likes `games` and y is the specific
       project like `pokemon_map`.
* Check public, private, "package private" for attributes and methods.
* If there are objects that have too much functionality bundled into them, 
  but they should be refactored into multiple smaller objects, make this observation,
  and add issues for it.
* If the point estimates are too low in your opinion, you may change them.


# Common Problems with legacy code repos

## Moving JUnit jar into /lib subdirectory

You may find that many old projects have ant tasks that depend on a hard coded location for the JUnit Jar that only works on CSIL, namely: 

 /cs/faculty/pconrad/public_html/cs56/lib/junit-4.8.2.jar

For example:

<pre>
  <classpath>                                                                                             
     <pathelement location="/cs/faculty/pconrad/public_html/cs56/lib/junit-4.8.2.jar"/>              
 </classpath>         
</pre>

This might or might not be factored out, so you may encounter this in multiple places throughout the file.   Which brings up: this is as good a time as any to [[Ant#Factor_out_my_classpath.3F|factor out your classpath]].

This hard coded path only works if you are compiling on CSIL.  The aim is to have the github repos be independent of any particular computing environment, and self-contained.

So, instead, you should create a lib subdirectory in the main directory of the project (i.e. the main folder in which the github repo is based) and download the JUnit jar file into that subdirectory:

 mkdir lib
 cd lib
 wget http://www.cs.ucsb.edu/~pconrad/cs56/lib/junit-4.8.2.jar

You'll need to add the junit jar to the github repo.  This may require the use of the -f option to "force" the add, since .jar files are likely in the .gitignore:

<pre>
-bash-4.2$ git add junit-4.8.2.jar 
The following paths are ignored by one of your .gitignore files:
lib/junit-4.8.2.jar
Use -f if you really want to add them.
fatal: no files added
-bash-4.2$ git add -f junit-4.8.2.jar 
-bash-4.2$ 
</pre>

Ultimately, a better solution is use a tool such as Maven that automates downloading a locally cached copy of the  junit jar on demand right when it is needed.  That way, we don't have to store multiple copies of the JUnit jar file in dozens of repos; nor do we have to update each of those separately if/when JUnit has a version change. 

However, one step at a time.

Once the JUnit jar file is in the ./lib subdirectory, we can change the build.xml file accordingly:

<pre>
  <classpath>                                                                                             
    <pathelement location="lib/junit-4.8.2.jar"/>                                                   
  </classpath>            
</pre>

Note that you must specify: <code>./lib/junit-4.8.2.jar</code> or <code>lib/junit-4.8.2.jar</code> NOT <code>/lib/junit-4.8.2.jar</code>

Note that the first two are relative to the current directory (the base of your github repo where the build.xml file lives), while the latter is an absolute path based at the root of the file system.  It is unlikely that there is a lib subdirectory at the root of the file system containing the JUnit jar file.


== Removing unnecessary tasks ==

There may be a variety of tasks in the build.xml files left over from the Mantis days that are no longer necessary.    These tasks should be removed from the build.xml files as they are encountered.

Tasks to be removed include:


| task | old purpose | why no longer needed |
|------|-------------|----------------------|
| publish | ran tasks to generate javadoc, build website, and put downloadable files on the web | we now publish via github |
| download | ran tasks to generate zip, jar and tarball (.tgz) files to put on the web |  github is now where downloadable code can be found |
| dist | ran tasks to generate zip, jar and tarball (.tgz) files to put on the web |  github is now where downloadable code can be found |
| jws | ran tasks to generate files for java web start | jws is not in common use  |



== Tasks to be retained/updated ==

Do not remove tasks that still serve a useful purpose.  Tasks you should keep include the following.  Note that some may require modification:



| task | purpose | why still needed |  modification that may be needed |
|----|--------|---|----------|
| compile | compile the code | most basic function of an ant build.xml file | change classpath if it is using hardcoded JUnit jar file from CSIL (migrate to ./lib subdirectory--see instructions above) |
| jar | create a jar file from the project | having a jar file of the project is still quite handy for distributing binary versions, and for running easily with command such as: <code>java -jar blah.jar mainClass</code>  | jar file should go into separate ./dist or ./build directory, but should be "cleaned" by the clean task--it is a temporary file in the same way that contents of build directory are. |
| javadoc | Create javadoc for the project | We still want javadoc for our projects | Should go into a temporary javadoc directory.   Remove code that refers to a URL if that URL is hard coded to be on www.cs.ucsb.edu.  Instead, we'll use a gh-pages branch and publish to github pages |
| clean | cleans up temporary files | still needed, especially before doing a <code>git status</code> or <code>git add</code> or <code>git commit</code> | check to see if directories listed are still being created by any tasks.  For example, if all other tasks referring to the download directory have been removed, then the <code>download</code> directory no longer needs to be a part of the <code>clean</code> task. |

== Fix 'includeantruntime' warning ==

Run ant compile and if you get this message:

```
 warning: 'includeantruntime' was not set, defaulting to build.sysclasspath=last; set to false for repeatable builds
```

Add an issue to fix this.   (TODO: Insert link to instructions)


# ant -p

Run this command:

<pre>
 ant -p
</pre>

Do you see descriptions for each ant target?  What you want to see is something like this:

<pre>
-bash-4.2$ ant -p
Buildfile: /cs/faculty/pconrad/github/cs56-utilities-ldap/build.xml

Main targets:

 clean       clean up project
 compile   compile code
 jar            generate jar file in dist directory
 javadoc   generate javadoc in javadoc subdirectory
 run           Runs a simple query
Default target: compile
-bash-4.2$ 
</pre>

If instead, you see something like this, then it means the ant targets lack proper descriptions:

<pre>
-bash-4.2$ ant -p
Buildfile: /cs/faculty/pconrad/github/cs56-utilities-ldap/build.xml

Main targets:

Other targets:

 clean
 compile
 jar
 javadoc
 run
Default target: compile
-bash-4.2$ 
</pre>

To add them, change this:

   `<target name="compile" >         `

to this:

   `<target name="compile" description="compile code">        ` 

This may seem annoying and redundant, especially for ant targets where the name is self-documenting.    The thing is, adding a description is a signal that this target is a "main" target, i.e. something that end users might actually type after the word <code>ant</code>, as opposed to targets that are just "internal" targets used by other targets.  Having&mdash;or not having&mdash;a description on your targets is sort of like the difference between "public" and "private" methods in a class.

