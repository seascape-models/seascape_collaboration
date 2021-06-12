# The general framework for collaboration in the Seascape models Lab

Max Campbell, Chris Brown, Christina Buelow

## Quick links

[Get directory template](https://drive.google.com/drive/folders/1dCdiRN_8FS5AD5XSGm9nlPYaxtmwZXSE?usp=sharing)

[Quick how to guides](/tips-and-guides.md)

## The Motivation

This framework was designed for the seascape model lab to be able to collaborate across multiple projects with a consistent and coherent structure. To effectively use this framework you need to have a basic idea of git, GitHub, folder directories and Google Drive. We can teach you if you don't.  

The figure below explains the framework. Ask us if its not clear.

The orange box lives only the internet, purple box lives on the internet and maybe somewhere else if working offline, and the blue boxes can live anywhere (but we recommend they live on the google drive too). The green arrows indicate transfer of information/files/data. Note that GitHub and Google Drive are not connected in any way (and they operate completely independently). **NEVER** share your user folder with another user whom is connected to the GitHub repository or you may **LOSE YOUR DOCUMENTS OR CODE**.

![**Figure 1**. The general framework of collaboration in the Seascape models Lab.](Outputs/proposed_collab_framework.png)

## TODO List

* Present to lab @maxcampb
* Get other opinions on what works well with collaboration
* Workshop at GC
* Online workshop?
* Ensure that everyone is familarised with the framework


## Google drive (storing data)

Google drive is a cloud-based storage that works very similar to a giant USB drive which is backed up online. The trickiest part of using google drive is making sure that you are set up properly on your personal computer ([read here]( https://support.google.com/drive/answer/7329379#zippy= )). After this is done it should work just the same as any other directory (folder structure) with a few extra Google drive options.

* Suggest you save project here along with data, but **ONLY SHARE THE DATA**.
* Students and Staff seem to have unlimited Google drive storage until further notice.


## Git

Git is a “version control” system. This system saves old versions of your project, text, and code. For a beginner user it is sufficient for you to just check that you have at .git file in your project directory, if you do, you don’t need to worry about anything further. Each project needs its own .git file and this should be located at the highest level in the project directory.

The .git file keeps track of all the changes made to each file in the folder, so you can 'go back in time' and recover old versions.

## GitHub

Github is a cloud-based storage system that stores the contents of your Git repository online (**MAKE SURE YOU HAVE THE REPOSITORY SET TO PRIVATE IF DESIRED**). Our lab, interacts with the content of the GitHub in two ways, using the desktop app and using GitHub in your web browser.

You also need to ensure that you have a GitHub premium account (this is free for students).

Maximum file size is 100mb. Recommend that entire project is less than a 1gb (use private folders or OLD – see explanations in Directory Templates section)

You need to be able understand and do the following by yourself.

* Commit – Save changes of your project to .git file in your local computer/cloud directory
* Push – Send changes to GitHub so others can access them and update their project version
* Pull – Update the project on your local computer/cloud directory with changes others have send to GitHub
* Clone – Bring an already existing project down to your local computer/cloud directory (you would do this when joining or continuing someone else’s project)
* Invite – Add another user to your project so they can make edits, join or continue with your progress.


## Directories and files

Directories are hierarchical structures for storing information (folders in folder in folders). Shortcuts allow you to jump between paths. There are some differences in the general directory structure of MAC and Windows, so you need to be aware of the ones relevant to your operating system (see below for details). The main thing you need to understand here is the structure of a directory. We stress on proper usage of sub-folders (do it smart not lazy so directories are easy for another user to understand).


#### MAC
Your main folders and files should stem from the Users folder. You can navigate through the directory using the “/” operator. For example, “/Users/maxcampbell” is the location of the base directory for the user “maxcampbell”, further if we want to go lower in the directory “/Users/maxcampbell/Documents” will take into the “Documents” folder of this user “/Users/maxcampbell/Documents/Active_projects” into the “Active_projects” folder within the “Documents” folder of the user. Finally, if wanting to refer to the data saved as at csv file in the “Active_projects” folder we use “/Users/maxcampbell/Documents/Active_projects/data.csv”.  And you should be able to access any file on your computer using this method (including a folder on Google Drive, after you have the Google Drive app).


#### Windows
Your main folders and files should stem from the Users folder. You can navigate through the directory using the “\\” operator. For example, “C:\\Users\\maxcampbell” is the location of the base directory for the user “maxcampbell” , further if we want to go lower in the directory “C:\\Users\\maxcampbell\\Documents” will take into the “Documents” folder of this user “C:\\Users\\maxcampbell\\Documents\\Active_projects” into the “Active_projects” folder within the “Documents” folder of the user. Finally, if wanting to refer to the data saved as at csv file in the “Active_projects” folder we use “C:\\Users\\maxcampbell\\Documents\\Active_projects \\data.csv”.  And you should be able to access any file on your computer using this method (including a folder on Google Drive, after you have the Google Drive app).

![**Figure 2**. An example of the hierarchical nature of directories on a user’s computer. Red path shows the example we gave in the directories operation system section. Teal paths indicate an example of a project directory.](Outputs/Directory_example.png)

#### Naming files and Directories

For tips on naming things we follow similar [Jenny Bryan's naming protocal.](http://www2.stat.duke.edu/~rcs46/lectures_2015/01-markdown-git/slides/naming-slides/naming-slides.pdf)

This includes:
* Using logical (e.g. start with "001_" to signal step 1, and  "002_" to signal step 2.) rather than chronological order (do not use dates because they have to constantly be updated and are not very human-readable).
* Descriptive names
* Using "-" and "_" to separate words
* No special characters
* "**-v2**.csv" style to signal new versions and count up numerically (throw old ones in the OLD folder)


## Documenting changes

One of the most crucial parts of collaboration is documenting the relevant project information. We do this in two ways using the Materials folder and IMPORTANTLY using a README file. The Materials folder contains interesting content that you have found or made (such as excel spreadsheets, bits of writing, key emails, papers, etc.). Whereas the README file has a summary of the most important project information (you could pretty much copy this in the methods sections of a manuscript as a starting point). Another KEY part of a README file is that it contains a TODO (to do list) at the very beginning so it is easy for you or someone else to pick up a project where you have left off. This README file should be an .md file so we can easily view it on GitHub.

Often, we think of recording metadata (project information) as being a painful exercise and we often tend not to do enough of it. So, my tip would be UPDATE THE TODO SECTION OF THE README EVERYTIME before leaving the project for any reasonable period of time, this will take a short period of time and save you and your colleagues many hours of confusion in the long run. And additionally, update the rest of the README every now and again, when you are feeling motivated (this will pay off when it comes to writing the paper).

You can edit the README.md in any text editor, though I like R studio.

## Using issues

Github issues allow us to be able to keep track of things that need to be resolved, record potential bugs and highlighting document checks needed, while assigning responsibility to the task to a person. These issues are a good place to have discussion on a particular issue by using commenting (this way we can keep track of the juicy details).

These should be written directly in GitHub.com (COMMAND + I in the desktop app) or on the mobile app. Note that you can assign parts of an issue to a users using "\@username", and make a checkbox in th use using "- [ ]".

After creating an issue make sure that you delegate at least 1 assignee who is in charge of making sure that the issue is addressed (if unsure who to assign, assign yourself), and add relevant labels.

#### Creating and removing an issue

1. Go to the ![GitHub.com](https://github.com/)
2. Move to the relevant project repository.
3. Click issues, and then new issue.
4. Fill in the details of the issue (using checkboxes "- [ ]") and assigning sub-parts of the issue to the relevant user using the "\@" operator, and then submit the issue. Create the issue.
5. Make a user an assignee (they are now in charge of the issue)
6. Wait till issue is resolved ...
7. Close the issue when it is resolved.
8. Hooray issue solved!

## Using discussions

In addition to using issues we use discussions. Where important distinction between an issue and a discussion is that issues are tasks assigned to individuals or groups which are expected to be completed, while participation in discussion is welcomed but not essential. Think of discussions as a way to share thoughts, get help, help others and network. The advantages are:

* Not having to answer the same questions multiple times (people can be referred to the discussion)
* Efficient usage of lab expertise
* Great way to learn passively and actively
* Easy way to get feedback
* Networking opportunity

Please follow the guidelines below when participating in discussions, and use the following flow chart.

#### Discussion guidelines

Please adhere to the following when using discussions.
* First diagnose whether this material is appropriate for a discussion using Figure 3.
* Do not tag or target other users in the discussion (if you want someone specific to answer ask them politely on teams).
* Never put down others.
* Make SURE you mark as answered after you question has been answered, to avoid wasting other users time. And do NOT delete discussions after they have been answered, because they may inform other users.
* Upvote and like good responses.
* We encourage answers from everyone because they give us a chance to learn, however, please attach a level of certainty to your response on a scale of 1-10 (where 1, 5, 10 are 10%, 50%, and 100% sure respectively). For example a response might be "That you sea surface temperature is the most important factor according to the literature (6/10)." or "Use an ANOVA not Kruskal wallace test because your residuals are normally distributed (8/10)."
* Do not ask about personal matters here.
* Make sure that the questions are self contained (have adequete information contained to solve).
* Make sure your answers contain enough detail to make sense.

![**Figure 3**. Diagonosis of a discussion or issue.](Outputs/Discussion_flowchart.png)

#### Other types of discussions

**Q&A:** These are the main type of discussion and should have solution.

**Announcements:** These are lab wide announcements, that should be read by everyone.

**General:** These are general back and forth discussions that have no clear answer. For example, discussing how to respond to reviewer comments, how to interact with an organisation or professional advice.

**Ideas:** These can be used to discuss future direction of research or improve projects.

**Show and tell:** These are for communicating something you have learn to the lab.


## Directory templates

Several templates have been made for your convenience, access them [here](https://drive.google.com/drive/folders/1dCdiRN_8FS5AD5XSGm9nlPYaxtmwZXSE?usp=sharing) (descriptions on contents below).

The project folders contain some of the following (with description):
* README.MD (standardised Rmarkdown file – see Documenting Changes section)
* Manuscripts/ (folder to store your project manuscripts)
* Materials/ (folder to store meta data and useful writing)
* Data/ (folder to store all data. This should live on the cloud and be shared with collaborators)
* Figures/ (folder to store figures from analysis or other)
* OLD/ (folder to chuck OLD stuff in found in several directories)
* Private/ (Things you do NOT want to end up on github or share with other users, e.g. large files, personal files etc.)
* .git (hidden file which does version control)
* XYZ.rproj (open R by clicking on this, which sets working directory in R)
* .rprofile (hidden file, to change if data lives elsewhere – see Advanced usage)
* .gitignore (hidden file tell the .git file what should be recorded and should be shared online through GitHub – see gitignore for further details)

![**Figure 4**. A visual representation of how an operation project should be structured that uses R (starting with the R_project_START).](Outputs/folder_structure.png)


## Compatibility with R

This framework was designed to work particularly well with R, but will also work well with other programming languages.

* Use R projects for convenience
* Understand how to change work directories easily in R
* Personalised .Rprofiles to find the data if in different location to scripts (e.g. the spatial drive), see advanced section below

## Using the mobile app

This application lets you look at code, issues and get notifications. You can also create new issues from your phone, however, some functionally seems to be reduced. Either way its cool so give it a GO!

## Advanced usage

#### Markdown and HTML

* Learn how to use markdown, [here are some tips](https://rmarkdown.rstudio.com/lesson-1.html)
* For code write using:

\`\`\`r

My r code here

\`\`\`


#### LATEX compatibility in R markdown and markdown

* Mathematics equations are great in LateX see guide [here](https://oeis.org/wiki/List_of_LaTeX_mathematical_symbols)
* Can use them directly in R markdown with "$$ your latex for separate line $$" or "$ your latex for inline $"
* If wanting to use in github discussions need chrome attachment [purple pi](https://github.com/nschloe/purple-pi)

#### .gitignore

.gitgnore files are to stop git from commiting files with certain extensions. These files will never be synced online. You can change this file if desire. To understanding the patterns ignored in the git file [read here](https://git-scm.com/docs/gitignore).

#### Git branches
These allow you to make changes to the project that you may or may not want to include in the future (think of them as the same project in a parallel universe). The big downside is that it is that you need to have a fairly good understanding of GitHub to use and that it becomes more difficult to predict how changes on the main project will be integrated with the branch in the future.
* Don’t recommend using these unless you know what you are doing
* They can be really useful if you want to trial substantial changes that you will want to keep or not in the future
* Or if you want to take several directions on the same project

#### Storing data somewhere else such as the spatial drive

If using R:
Write a function in the project .Rprofile file the adds the appropriate working directory to a file path. The .Rprofile is run when you open the project so you will always have access to the function if you opened the R project.

Function below to add extention to filepath x (e.g. x = “Data/data.csv”). Check Sys.info()["user"] for your computers user.

```r
mpath <- function(x){

  if (Sys.info()["user"] == "maxcampbell"){
    max_ext <- "/Volumes/GoogleDrive/My Drive/tuna-bycatch-study/TNC Tuna Project/"
  } else if (Sys.info()["user"] == "s2989645") {
    max_ext <- "C:/Users/s2989645/Google Drive/tuna-bycatch-study/TNC Tuna Project/"
  } else if (Sys.info()["user"] == "ameliadesbiens") {
    max_ext <- "/Users/ameliadesbiens/Google Drive/tuna-bycatch-study/TNC Tuna Project/"
    } else {
      max_ext <- ""
  }

  paste0(max_ext, x)

}
```

If using another Program:
Set the appropriate working directory in the program (could use a similar function to above R version easily enough).

## Options (unresolved)

Google drive or Onedrive: I recommend google drive from limited reading, because apparently Onedrive occasionally mixes file (which would really suck!).

## Current limitations

* Naming convention of folders allows for potential problems with sharing the incorrect data and or files, and makes it easy to overwrite files
