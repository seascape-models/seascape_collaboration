
# Current limitations

* Naming convention of folders allows for potential problems with sharing the incorrect and or files, and makes it easy to overwrite files
* Binary files are not backed up on GitHub

## Options (unresolved)

Dropbox, Google drive or Onedrive: I recommend google drive (out of the free alternatives) from limited reading, because apparently Onedrive occasionally mixes file (which would really suck!). However, I still think Dropbox is the best of the three from my experiences.


# Risks and solutions


This document is designed to identify and document potential sources of problems to ensure that we are sufficiently prepared to deal with these problems should we run into them in the future. Note these are only the identified problems potentially feasible solutions and are not necessarily adequate solutions. Further not that the consequence and likelihood are further influenced by: the users expertise on the project, the size of the project, the structure of the project and current software in use. Thus, project risks should be considered within their individual context.

A general and important comment is **if the consequences could be moderate to extreme, and you do not feel like you do not have the expertise to resolve this issue yourself, step 1 should ALWAYS be ask for help from someone who has more experience. Otherwise, you might make matters worse.**

We base our ratings on the following risk assessment guideline
![**Figure 1**. Risk matrix retrieved from online](/Materials/Outputs/risk-matrix.jpeg)

## Cloud contents is corrupted of deleted

This would be in the case that the files on a cloud based system stopped working. Probably, this is not a massive deal because you should be able to access a previous version on a file. The consequences could be worse if the corruption or deletion affected the contents of the "Shared" folder, because that isn't backed up on GitHub (its also more likely because of the multiple users).

**Risk Range** = 2C - 3C = Medium 

### Potential causes

* .git file being corrupted?
* delays in syncing
* One of the users deleting something accidentally

### Mitigation strategies

**Currently implemented**

* Save frequently
* Back up files on active projects on you computer
* GitHub/.git have copies of scripts and many materials
* Make sure that you keep clean and well structured directories

**Potential**

* Save periodically on an external drive
* Periodically store important files not also backed up on GitHub

### Course of action (help)

1. See if you can retrieve files locally offline first (without updating from the cloud).
2. Try to retrieve files from the cloud system
3. Contact other users if this repository is shared and see if they can retrieve
4. Contact the cloud system provider for help
5. See if you can identify why this corruption or loss occurred and mitigate the risk for next time.
6. Once resolved replace corrupted files with uncorrupted files


## .git file is corrupted

This is noted as a common issue for using .git files with cloud based storage systems such as dropbox or google drive. In many cases people say do not not mix these systems, however, because the .git folders are saved to GitHub (Max and Eric think this is not really a problem in our framework). In the case where you have not pushed your changes to GitHub upon leaving a project, it is possible that you might loss these changes if the .git file was corrupted. Perhaps these changes could be retrieved to from the cloud system, but perhaps not.

**Risk Range** = 2D - 2B = Low to Medium 

### Potential causes

* Multiple users making changes to the same git repo at a similar time
* Using multiple computers (particularly if they are used at a similar time). This is OK to do but make sure you push your changes to GitHub before switching computers (**DO NOT RELY ON THE CLOUD SYSTEM TO SYNC YOUR GIT FILE CORRECTLY**)
* Cloud system not being up to date on its syncing

### Mitigation strategies

**Currently implemented**

* Push your changes to GitHub before leaving your computer, especially if you are moving to another machine
* Do not share .git files or folders that contain them with other .git users instead use GitHub (and our framework), or move to the shared folder or email chain not tracked by git.

**Potential**

* Keep git repo on local machine rather than on cloud based systems (this is messier).

### Course of action (help)

0. Be sure you know what you are doing here
1. Make sure all your files are synced properly to the Dropbox/google drive folder and append this folder name with "_corrupted"
2. Remove the corrupted git repository from the project folder.
3. Clone a new version of the git repository from GitHub to the dropbox, making sure you do not save over the "_corrupted" folder.
4. Manually replace the files that you have made changes to in the new version on the project folder (that you just cloned from GitHub), and add shared folders and those not tracked by GitHub
5. Check that the changes to commit make sense, **IF** they do you could commit them and push them to GitHub so they are safe.  


## Harmful push to GitHub

This would involve someone (probably accidentally) pushing something to GitHub that they should not. This could potentially result in us losing progress on something that we would have to either retrieve from a earlier version, break something that was working or potentially lead to us redoing something. This could create quite a mess as we might not notice that the changes had been made until the project had substantially progressed.  

**Risk Range** = 1B - 3E = Low 

### Potential causes

* Users not understanding the system properly
* Regular mistakes in code
* Careless work and pushes
* Intentionally harmful pushes (however unlikely)

### Mitigation strategies

**Currently implemented**

* Training and guidelines for users
* Maintainers should check code that is pushed to their repos fairly frequently 

**Potential**

* Use pull requests (this is secure but is more complex and time consuming)

### Course of action (help)

1. Discuss the push with the user who made the change to ensure that the change is not appropriate.
2. Revert to old version of the git and add any parts of the changes that you want to keep **OR** update the changes in their current state to ensure that they are appropriate. 

## Sharing the wrong folder

This could be harmful if the folder kept being shared while multiple users were working on files and/or pushing to GitHub (probably most like corrupting the git, but potentially worse). However, this is not a big deal if the users quickly notice and unshare the folder (so keep and eye out for this). The most dangerous cases would be when multiple users are working on the same files, where progress could be overwritten.

**Risk Range** = 1B - 3D = Low to Medium 

### Potential causes

* Poor understanding of the framework
* Carelessness

### Mitigation strategies

**Currently implemented**

* Quality training on using the framework
* Encourage extra vigilance while sharing
* Only share one folder (the shared folder)

**Potential**

* Period checking of which folders are shared

### Course of action (help)

1. Quickly unshare the folder that was not supposed to be shared
2. Notify the person you shared folder with.
3. Reshare the correct folder.


## Saving conficting versions of files

Two or more users making changes on the same file at the same time. Luckily, git handles conflicts really well, so it would be easy for one of the users to fix in this case. But, when conflicts are made within the shared file this could lead to changes being **LOST**, though this is really not different to current use of cloud systems. However, this is probably the most risky part of our framework, so it should be handled with care.

**Risk Range** = 2C - 3D = Medium 

### Potential causes

* Users working on shared files at the same time
* Users pushing changes without pulling previous changes
* Not saving your changes before you walk away


### Mitigation strategies

**Currently implemented**

* Notify other users when you are working on shared files
* Guidelines in the framework for working on shared files
* Save every time before you walk away from your work

**Potential**

* Have files locally and share every time (messy)

### Course of action (help)

1. If working with files tracked by git (those files not within the Shared folder), just resolve the conflict through the GitHub desktop app (not a big deal)

<br>

1. If working with files not tracked by git (Those in the Shared file). Retrieve both files from the history of the Cloud based system if you can.
2. Figure out which version of the file is more progressed. 
3. Manually update that file with the changes from the other file.

## Failure to pull before beginning work

If you have no conflicts this does not matter at all. If you have some you just need to resolve the conflicts.

**Risk Range** = 1A - 2B = Medium 

### Potential causes

* Poor understanding of the framework
* Carelessness

### Mitigation strategies

**Currently implemented**

* Quality training on using the framework
* Encourage going to the desktop app always before starting work

**Potential**


### Course of action (help)

1. As soon as you have noticed that you have forgot to pull, save you work and pull from GitHub.
2. Merge files and resolve conflicts if there are any through the desktop app.

## Switching computers before cloud finished sinking

If you were working in the shared folder and you continue to do so on your other computer, you could overwrite changes (and potentially lose progress). If working with files tracked by git you could corrupt the repository.

**Risk Range** = 2B - 4C = Medium to High 

### Potential causes

* Poor understanding of the framework
* Poor internet connection
* Careless ness
* Working offline

### Mitigation strategies

**Currently implemented**

* Risk awareness
* Quality training

**Potential**

* Manually sync before moving to a second computer

### Course of action (help)

See other risks and take the actions based on what the consequences of using the second computer were.

## Both the cloud system and .git breaking at the same time

This is potentially the worst thing that could happen, if both systems were to fail you would have to revert to an earlier versions of the work. Currenty, I cannot see how this could occur but it would probably be be some kind of complex interaction between the systems.

**Risk Range** = 2D - 5E =  Low to Medium 

### Potential causes

* Using multiple computers
* Strange software configurations

### Mitigation strategies

**Currently implemented**

* Encourage pushing to GitHub frequently and before you leave your work
* Save frequently

**Potential**

* Do not use git with cloud based storage (messy) 

### Course of action (help)

Get help unless you know what you are doing here, probably the best actions are somethink like:

1. Retrieve previous versions of project from the cloud storage system.
2. Clone a new project folder from GitHub
3. Replace files in the new project folder with those from the old folder that are more progressed, as well as adding any folders not tracked by git to the new folder