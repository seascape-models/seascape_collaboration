# Important Tips

## Measures to prevent problems

As with any framework there are [potential risks](limitations_risks_and_solutions.md) involved in using this framework. However, if you follow the below measures it is unlikely that you will have any issues, while using the framework.

1. The "Shared" folder has the same syncing flaws as using shared folders on dropbox/google drive. So you should make sure that you are not working on the same file as someone else in the "Shared" folder (let other users know when you are working on something that they might be).
2. Make sure that you save your work frequently while working on something, and **ALWAYS** when you leave your workstation.
3. Make sure that the cloud syncing process is complete before you leave your workstation, switch computers or allow others to work on the same files that you have been. Where, you should avoid working offline and with poor internet connections where possible.
4. Push your changes to GitHub before leaving your work station, **IF**, your push does not potentially damage other parts of the project (this is 99\% of cases) . **IF** your push may be harmful, **DO NOT PUSH**, save locally, and ensure that it is safe to push your progress ASAP (and then push).
5. Make sure that you move "Shared" folders to the correct location as soon as they are shared with you.
6. Do not share any folders other than the "Shared" folder.
7. Pull every time before you start working on the project.
8. If you get conflicts when pulling from GitHub, resolve them immediately before continuing.
9. Keep your folders clean and well structured.


If you have any issues while using the framework refer to the [risks and solutions document](limitations_risks_and_solutions.md) and seek help.

## Data management practices

Data management is often not given the priority it deserves in research science. This is often because we are driven primarily by research paper outputs, and we get mostly hidden rewards from having good data managment practices. We often will not notice the effects of poor data managment until its too late.

Here, are some examples of the good data management vs poor data management:

* We come to the end of our project and realise our files are a mess with lots of inconsistencies (poor data management) or remain well organised an easy to interpret (good data management).
* We lose some important files and are not able to retrieve them (poor data management).
* We can easily can share our code and data with collaborators and they can interpret it (good data management).
* We spend many hours over the course of the project looking for files (poor data management).
* We can publish our code without any hassels (good data management).
* When we stop using our data (or retire) others can either use and interpret our data (good data management) or the data is lost (poor data management).
* We come back to a project a decade later to use some code and data and either do this easily (good data management) or with extreme difficulty (poor data management).

The SCF is designed to help with data management, but without considering data management (before, during and after projects) you leave yourself open to being another victim of poor data management. Here are some resources for considering data management: a blog on the [top ten tips for research data management](http://blogs.nature.com/naturejobs/2014/11/25/top-ten-tips-for-research-data-management/) and [how to guides](https://www.dcc.ac.uk/guidance/how-guides) from the the Digital Curation Centre (DCC).


## Making code public

There is an increasing push to make scientific code public into the future this promotes honesty, transparency and good science. As researchers this can make us feel uneasy. We worry that our code isn't good enough, is messy and/or will have bugs. Nick Barnes, a professional software engineer, suggests that [our code is good enough](https://www.nature.com/articles/467753a). Publishing your code is a great contribution to the world of knowledge, because without sharing your code many of your findings, ideas and methods would be lost. Your code can inform the future work of others, and push forward humanity.

So next time you finish up your project, given that you authority to do so (i.e. talk amongst your collaborators), consider making your GitHub repository public or publishing your code somewhere else.

If you code is of appicabilty in a general sense consider making a realise or publishing a package.

## Collaborate outside of the lab

When collaborating outside the lab you have a few options that we recommend. Any of the below options should work fine.

* Encourage your collaborator to use the SCF, adding them to the GitHub repo and only sharing the "Shared" folder (the most secure way).
* Add them to the GitHub repo and don't share anything with them on cloud storage folder. Instead, zip any data they need and send to to them, via email or on cloud (this is very secure albeit a bit messier).
* IF THEY DONT USE git/GitHub you can share the folder with them via the cloud storage (Realises on cloud storage syncing). You will still be able to use the SCF with other collaborators but make sure you know how you are collaborating with each user.
* Zip the entire project and send a copy and manually update as you go (very secure but also very messy).

# Other tips and tricks

* Use “_” instead of space in folder names
* Have your OS display hidden files
* Get a spell checker for Rstudio
