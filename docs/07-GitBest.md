# GitHub Best Practices {#Best7}



Now that you have a GitHub account and are set up on GitHub Desktop or RStudio, we will bestow upon you some additional best practices.

## Use a unique repository for each project {#Best7.1}

You can host multiple projects on GitHub at the same time but it would be a mistake to use one repository to store information about multiple projects. Make sure you maintain a unique repository for each project. Like folders on your computer, this will keep your code organized and your brain happy.

## Use branches to avoid heartache {#Best7.2}

As you learned in [Chapter 5](#Branch5) a `branch` is a way work on alternative versions of your scripts (e.g., a new feature or modification), while not affecting the original (i.e., the main or default branch). It is good practice to work on short-lived branches, so that merging is easier and so that you are not risking breaking what is already working!

## Create a meaningful `.gitignore` file {#Best7.3}

`.gitignore` files are plain text files that instruct the program on predefined files that should be ignored.

Specifically, GitHub has a file size limit. It is therefore best suited to storing your R scripts and other related files (e.g., `README`), **but not raw data and large output files**. These files should be save elsewhere on your computer and *backed up* on your cloud storage. This also allows you to share scripts publically, but to keep potentially sensitive data separate.

Recall that during the creation of your first `repo` we selected the R `.gitignore` file template, which will be saved in your root folder. You can open this file in RStudio and add or remove any file types.

For example:

`.pdf` `.csv` `.xlsx`

## Define the code owner {#Best7.4}

It is important that you give yourself credit for the code you create, and likewise give others credit for the code they created. If you borrow or modify code from another source, this is OK! Just make sure you give credit where credit is due. Similarly, if you are collaborating on code development, define the roles of each author. This can be done at the front end of your scripts and interspersed within the script.

GitHub has a built-in code owners feature that allows you to grant access to a particular group of staff or partners. Only verified code owners will be able to edit or review the project. The code owner feature can be used for more than assigning individuals to work on the repository. It can automatically assign teams and grant them permission to work on the project and maintain the repository. Birds Canada will be using the team and code owner feature to manage scripts that are shared.

## Don't let your password leak into your code {#Best7.5}

While it seems obvious that you should not share your password, you might accidentally save this in your source code and `commit` it to GitHub. For example, when downloading data from NatureCounts using the R package, you might be inclined to save your username and password in your source code. Ensure this isn't the case before you `commit`!

## Don't commit a crime {#Best7.6}

Make small commits and make them often. Each commit should reflect changes that are easily accompanied by a single and informative commit message. For example:

-   "Change made to analysis model fit code"

You should try to refrain from making a lot of changes to a lot of sections of your code making a mixed-commit. For example:

-   "Major changes to analysis, data manip, and bookdown yml."

If you need to revert any files, or even just check your history of file changes, you will be happy you made consistent and well detailed commits.
