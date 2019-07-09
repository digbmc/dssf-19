# Sandbox

For the relevant commands, see your cheatsheets for [git](https://education.github.com/git-cheat-sheet-education.pdf) and [markdown](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf). If you need help, consult the [glossary](sections/glossary.md) your peers or the [answer key](sections/answers.md).

## Setting up

1. Start by **Config**-uring your name using the command line.
2. **Clone** this repository and open it in **atom**
3. Use the


## Publishing

1. Create a new markdown file in the documents folder within your local repository (the dssf-19 directory). Use the .md file extension.
4. Open the document in **atom** and write content using markdown syntax. Include headers, lists, text, and links or images.
3. Check your work in atom using the markdown preview package.
2. Save your new document
2. Check the **status** of your local repository according to git.
3. **Add** your document to git's plate so it knows you've made changes (also referred to as "staging" your changes)
4. **Commit** to the changes you've made (at least for now) and write a note about what you changed
5. **Pull** in any new changes from the cloud-based or "remote" repository (always do this before you push your changes to a shared repo)
5. **Push** your changes to the remote repository.
6. Open the remote in your browser to see what happened.

## Collaborating

1. **Pull** your teammates' changes. Look at the folder to see what happened.
2. Choose a new file added by a teammate (make sure nobody else is editing it  for now). Open it in Atom and make some changes to it.
3. Check the **status** of your local repo.
3. **Add** your changes.
4. **Commit** your changes with a message.
4. **Pull** any new changes, then **push** your changes to the remote repository.

### Extra credit

1. Now things will get more complicated. Open the file [collaboration.md](sections/collaboration.md) in Atom, make some changes, and save the file.
3. **Add** your changes and **commit** them
2. Create a new **branch** of the repository so your changes won't interfere with anyone else's work.
3. **Checkout** your new branch (switch to it).
4. **Push** your changes to your personal **branch** (you don't need to pull because nobody else should be working on this branch): git push origin [yourbranch]
5. Look at the remote in the browser and see if you can figure out where your changes went.  
6. Once you feel good about the changes you've made on your branch, you can try to **merge** it with the master branch.
