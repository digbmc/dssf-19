# Basic git workflow

Make sure you have a command prompt window open and that your current working directory is the dssf-19 repository. This is effective if you are the only person working on a repository or when (as is the case right now) each person is working on a separate document.

## 0. Save

Make sure you have saved changes to your file.

## 1. Stage or add

Before you can publish a file to GitHub, you have to tell Git about the file so it can track its changes. This is called "staging."

`git add newfile.md`

 If you'd like to add all recent changes at once, use:

`git add --all`

In atom, you can do this by opening the GitHub pane (Packages --> GitHub --> Toggle Git Tab)

![Atom toggle git tab screenshot](images/git-tab.png)

A column should appear on the left side. In the top of the column, you'll see a list of all the files in this repo that have "Unstaged Changes." To allow git to track them, click on "Stage All".

![Unstaged changes in Atom](images/unstaged.png)

Now you should see the same files listed under "Staged Changes".

![Staged changes in Atom](images/staged.png)


## 2. Commit

Once Git has begun tracking your file changes, you **commit** them: you package them for publication and label them for your collaborators, including your future self. Think of it as temporarily "committing" to a draft or a batch of edits.

`git commit -m "message describing my changes"`

In Atom, write a short message in the box below your Staged Changes. Then click "Commit to master."

![Committing in atom](images/commit.png)

## 3. Push

When you're collaborating with others, make sure you are working on the most up-to-date version of your repository by "pulling" any new changes from the remote to your local.

`git pull`

You can also check the status of your repo in relation to the remote (and your uncommitted changes using

`git status`

In Atom, you can check to see if there are updates to pull by clicking  on "Fetch" on the bottom of the window: ![fetch](images/fetch.png) If there are changes, you will see "Pull". Click to

Now that your colleagues have published their texts to github, pull them from the remote repository, then look at your local repository in finder. Can you see what happened?

## 4. Pull

Now you're ready to publish or 'push' to the remote repository and publish your changes to GitHub.

`git push origin master`

If you haven't yet contributed to GitHub from the command line, you will need to log in with your GitHub credentials.

In Atom, you'll see a list of your commits below the "Commit" button. If you have unpushed commits, you'll also see "Push" on the bottom of the window.

![pushing in atom](images/push.png)

Once you've successfully pushed, open the live site in your web browser: https://tri-cods.github.io/Ed-Minimal-Editions/

You may need to wait a minute or two, but your text should soon appear in the list of texts on the front page. How did that happen? Jekyll magic!


---

# Collaborating on GitHub

When you have multiple users contributing to a repository at the same time, using branches is one way to help minimize conflicts. Branching creates a personal version of the repository that you can make public without interfering with anyone else's changes. Once you are ready, you can merge your changes with the primary or "master" branch. At this point, any conflicting changes can be resolved.

Our next task is more complicated and will require simultaneous editing: you're going to add your name and a short bio to the [contributors page](https://github.com/tri-cods/Ed-Minimal-Editions/blob/master/contributors.md). You could do this by contributing directly to the master branch (as you have been doing), but if you all do that at the same time we are likely to encounter conflicting changes. Creating branches is one way to minimize these conflicts.

If you create your own branch and commit your changes to that branch, we can later review the various branches and merge everyone's changes.

In Atom, you'll see a branch icon labeled "master" at the bottom of your Git pane.

![atom master branch](images/branch.png)

This icon allows you to switch between branches or create a new branch.

![atom new branch](images/new-branch.png)

Note: Switching between branches will change your working tree to the version of the project represented by that branch, which may be ahead or behind the master branch. Make sure you've committed any new changes before you switch branches.

Once you have created a branch, you can commit changes to that branch instead of the master branch. Before these changes will be reflected in the remote repository's versioning, you must publish the branch by clicking "Publish."

![committing and publishing to a new branch](images/publish-branch.png)

Open the repository in your browser and try to find where your changes went. When you're ready to incorporate your changes back to the master branch, submit a Pull Request.

![GitHub branches](images/github-branches.png)

This will compare your branch with the master and determine whether there are conflicts that need to be managed.

![GitHub pull request](images/pull-request.png)

If there are no conflicts, you can easily merge your branch with the master.

![GitHub merge](images/merge.png)

If there are conflicts between the branches, you'll have to decide how to resolve them. After you've merged, you can delete your branch, or continue working on your branch.
