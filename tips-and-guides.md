# Important Tips

## Measures to prevent problems

As with any framework there are [potential risks](\limitations_risks_and_solutions.md) involved in using this framework. However, if you follow the below measures it is unlikely that you will have any issues, while using the framework.

1. The "Shared" folder has the same syncing flaws as using shared folders on dropbox/google drive. So you should make sure that you are not working on the same file as someone else in the "Shared" folder (let other users know when you are working on something that they might be).
2. Make sure that you save your work frequently while working on something, and **ALWAYS** when you leave your workstation.
3. Make sure that the cloud syncing process is complete before you leave your workstation, switch computers or allow others to work on the same files that you have been. Where, you should avoid working offline and with poor internet connections where possible.
4. Push your changes to GitHub before leaving your work station, **IF**, your push does not potentially damage other parts of the project (this is 99\% of cases) . **IF** your push may be harmful, **DO NOT PUSH**, save locally, and ensure that it is safe to push your progress ASAP (and then push).
5. Make sure that you move "Shared" folders to the correct location as soon as they are shared with you.
6. Do not share any folders other than the "Shared" folder.
7. Pull every time before you start working on the project.
8. If you get conflicts when pulling from GitHub, resolve them immediately before continuing.
9. Keep your folders clean and well structured.


If you have any issues while using the framework refer to the [risks and solutions document](\limitations_risks_and_solutions.md) and seek help.


## Collaborate outside of the lab

TBA ....

* What to share etc.
* What not to share


# How to do (guides) ...

### Starting a new project

1. Copy paste the desired project folder from the “seascape_collaboration folder” to the desired location on your machine (recommend this is on the google drive directory) and rename both the folder and the Rproject. And put files in relevant locations.
2. Link to GitHub, MAKE SURE YOU MAKE A PRIVATE REPOSITORY IF REQUIRED
3. Invite collaborators to join project on GitHub
4. Share data with collaborators from google drive
5. Update the README.MD
6. DONE

### Joining someone’s project (cloning)

1. Accept invitation to join repository on GitHub
2. Open the GitHub desktop app and clone the repository to the desired location
3. Add the shared data from google drive to the desired location
4. DONE

### Project workflow (from GitHub desktop App)

1. Click “fetch origin” to get the most up to date version of the project from GitHub (Pull request)
2. Make changes to the project just as you would on your local machine
3. Commit changes after filling out the summary description boxes
4. Push changes back up to GitHub
5. DONE

### Creating and removing an issue

1. Go to the ![GitHub.com](https://github.com/)
2. Move to the relevant project repository.
3. Click issues, and then new issue.
4. Fill in the details of the issue (using checkboxes "- [ ]") and assigning sub-parts of the issue to the relevant user using the "\@" operator, and then submit the issue. Create the issue.
5. Make a user an assignee (they are now in charge of the issue), and choose the correct labels (INCLUDING A PRIORITY).
6. Wait till issue is resolved ...
7. Close the issue when it is resolved.
8. DONE

### Mark and show lines of code within an issue

1. Go to the lines of code in question.
2. Click the first line of code you want to reference, then hold the shift key and click the last line of code.
3. Click on three dots to the left of code and select either "Copy permalink" and paste this in an existing issue or discussion OR "Reference in a new issue" to create a new issue with the code.
4. Fill in the rest on the details of comment or issue and submit.
5. Done

### Converting existing projects to the framework

**If they are complex and almost finished then don't do it. If they are simple and just started then move them.
If the are complex and have a long way to go move them (it will be easier in the long run).**

1. Copy a relevant project folder template from the [directory templates](https://drive.google.com/drive/folders/1dCdiRN_8FS5AD5XSGm9nlPYaxtmwZXSE?usp=sharing) to the relevant location on your computer.
2. Rename the folders and add new ones where needed.
3. Populate the new project folder by copying the contents of the existing project into the relevant location.
4. Store the existing (old) project in case it is needed in the future.
5. MAKE SURE the .gitignore folder is updated if you are NOT using the standard names.
6. Add new project as an "Existing repository" from the GitHub desktop app.
7. Publish repository on GitHub from the desktop app.
8. Invite other collaborators to the repository on GitHub in browser.
9. Share the data with other collaborators through data storage system.
10. DONE

# Other tips and tricks

* Use “_” instead of space in folder names
* Have your OS display hidden files
* Get a spell checker for Rstudio
