# HOW TO UNDO - Intro to Git and GitHub for Non-Coders

_How to use these essential free tools to manage projects, share content, and collaborate, all while keeping a record of versions and changes made along the way._

---

Git is a free and open-source version control tool that is widely used for working with code, and one of the essential tools enabling open-source collaboration.

While built for programmers, Git is an amazing tool that anybody can use to manage any kind of content.  Be it text, spreadsheets, images, vector drawings, or 3D models, you can put pretty much anything you want into a Git repository. Doing so will, almost like magic, allow you to easily manage versions of files, share and collaborate on them with your colleagues, create backups, and more.

Using Git you can, for example:
- Publish project documentation
- Manage versions of graphic design work such as posters or fliers
- Make a repository of assets such as logos or icons
- Organise, backup and synchronise your notes across different devices
- Create a Wiki for your community

Whilst simple to use, Git can be confusing for new users, especially for those who are not necessarily interested in using it for software development, as most tutorials and reference material is designed for learning to use Git with code.

In this hands-on workshop, you will learn all you need to know to start using Git to organise your projects, and to publish and collaborate on them using GitHub.

Whilst this workshop is aimed at people with no programming experience, coders are also welcome to participate :)

Topics covered:
- Installing and using Git, GitHub Desktop and Obsidian.
- Writing in Markdown.
- Using Git locally.
- Collaborating on a repository using GitHub.
- Publishing a simple website using GitHub Pages.

_The workshop will be in English._

---

## Outline

_welcome and introductions_

- [Introduction]
	- Workshop outline
	- Git terminology, Version Control, Git background, GitHub and other Git hosting services.

- [STEP 1.1] Install Git
	- https://github.com/git-guides/install-git
	- Check if it is already installed with `git version` in the terminal
	- MacOS - Install using Homebrew
	- Windows - Download and install Git for Windows
- [STEP 1.2] Install GitHub Desktop, our "Git GUI Client"
	- https://desktop.github.com/
	- Temporarily set `name` and `email` to anything you like

- Your First Repository
	- Make a new repo with a README called `learning-git`.  Have a look at the folder this creates for you.
	- Make sure your file manager is showing hidden files, to see the `.git` folder.
	- Open `README.md` in a text editor (Notepad, TextEdit, etc...), and give it a nicer title and summary sentence.
	- In GitHub Desktop, make a commit and see how this appears in the history tab.
	- Make a new file in the text editor, write a todo list and save this as `todo-list.md`.  Edit README and make a note of the to do list as well.
	- In the GitHub Desktop, make another commit and give it an appropriate summary message.
	- Add any other notes you'd like to the readme file, under a **Notes** section, or make a new file called `notes.md`
	- Note that you can always edit your most recent commit.  To change the commit message, right click on the commit in the history tab and select 'Amend commit'. To remove the commit select 'Undo commit', and all the changes from that commit will appear back in the 'Changes' tab.

- [Summary]
	- Commit, README files
	- What is Markdown?

- [STEP 2] Install Obsidian
	- https://obsidian.md/download
	- Select 'Open folder as vault' and select the `learning-git` folder.
	- Change the vault settings (see [obsidian setup](#Obsidian-Setup-for-GitHub-Compatibility)).
	- Add an "install and use Obsidian" task to the to do list, and add check boxes to the tasks.
	- Add a link to the todo list in the readme file.
	- In GitHub Desktop, notice that obsidian has added some new hidden files. To tell git to ignore these files, go to Repository > Repository Settings > Ignored Files, and enter `.obsidian`.
	- This will create a new file in the working directory called `.gitignore`. Make a new commit to add the file to the repository.
	- Note that as soon as make any changes in Obsidian, these will appear in GitHub Desktop.  There is no option to 'save' in obsidian, your files are always updated as you modify them.

- [STEP 3] Make a New Branch
	- In GitHub Desktop, in the 'Current branch' menu create a new branch called `sandbox`.
	- Make some changes to the readme file, and make a new commit called `testing the sandbox`.  Switch between the `main` and `sandbox` branches in the Current branch menu, to see these changes appear and dissappear in Obsidian. Continue to experiment in the `sandbox` branch.
	- Download the [workshop poster zip](https://github.com/tiago-rorke/how-to-undo/raw/main/how_to_undo_cartaz.zip) file and extract it into the `learning-git` folder.
	- Make a new commit and notice how GitHub desktop diff window shows different things for the different poster filetypes.
	- Try moving files around and renaming them, and see how this appears in the history after making a commit.

- Use checkout to go back to a previous version of the sandbox.
	- In the history tab, right click on the `testing the sandbox` commit, and select 'Checkout commit'.  GitHub Desktop will warn you about 'detaching the HEAD', select 'Checkout' to confirm.
	- In the `learning-git` folder, notice how the posters are gone.  In GitHub desktop.  In the 'Current branch' menu, it will say 'Detached HEAD'.
	- Select `sandbox` in the 'Current branch' menu to return our files to the latest changes we made.

- [Summary]
	- Branch, Checkout, HEAD and "detached" HEAD.
	- Be careful not to checkout when you have files open in a program that doesn't watch for changes to the file as you are working on it.
	- Binary vs text files in Git.  Note about file sizes when working with binary files.
	- GitHub image diffs.
	- Why is Markdown so great?
	- Look at the obsidian Markdown syntax reference.
	- Look at some other online Markdown editors.
	- How I use tend to use git to organise my projects.

_Pause to play with obsidian and learn some more Markdown syntax._

- [STEP 4] Backup `learning-git` to GitHub
	- Sign up to GitHub, then sign-in in GitHub Desktop (File > Options > Accounts).
	- Make sure you are in the `main` branch, and select 'Publish Repository' and publish as a private repository.
	- Access your notes on GitHub via the dashboard.

- [Summary]
	- Local vs Remote repository
	- Push

- [STEP 5] "Food to Fork" - add your own recipe to the repository to share
	- https://github.com/tiago-rorke/food-to-fork/
	- Clone the repository from GitHub (File > Clone Repository > URL)
	- Open as vault in Obsidian, and change the vault settings again. (Unfortunately this must be done each time you create or open a new vault).
	- Create a folder for your recipe, and put a new note in that folder.  Add any pictures you would like to include to that folder as well.
	- Once you are ready to publish the recipe, make sure you have committed all your changes, and have updated your local copy with `Fetch` and `Pull`.  If there are no conflits to resolve, you can publish with `Push`.

- [Summary]
	- Clone, Pull, Merge

- Fork the MILL Wiki to add some content to the Lisbon Makers Map
	- Fork the wiki to your GitHub account at https://github.com/MILL-LX/mill-wiki
	- Clone your fork of the wiki to a local repository on your computer.
	- Edit the src/pages/map.md file, and add a supplier to the list.
	- Make a commit and push it to your fork on GitHub.
	- On on your forked repository page, go to 'Pull Requests' and make a new pull request.
	- If your request is accepted and merged by the original repository owner, you will receive an email notification!

- [STEP 6] Make your own recipe webpage
	- On GitHub, make a new repository for your recipe, and initialize it with a README.md file.
	- In the repository settings on GitHub, go to 'Pages', and under 'Branch' select `main` and `/(root)` as the folder, then click 'Save'.
	- Clone your new repository to your computer with GitHub Desktop.
	- Copy your recipe folder from the "food-to-fork" repository to your new repository.  Delete the existing readme file and rename your recipe file to README.md.
	- Make a commit and push it to GitHub.  After about 30s or so, your website will be online, you can find the link to it at the top of the Pages section of the repository settings on GitHub.


## Obsidian Setup for GitHub Compatibility

In `Settings`

 - `Files and Links` >
	- `New link format` - set to `Relative path to file`
	- disable `Use [[Wikilinks]]`
 - `Editor` >
 	- `Strict line breaks`



## Glossary

`repo`
`add`
`stage`
`commit`
`checkout`
`push`
`pull`
`fetch`
`branch`
`merge`
`diff`
`fork`
`clone`
`revert`
`rebase`
`stash`
`tag`
`origin`
`remote`


`version control` / `source control`

`distributed version control`


---

## Links

https://github.com/git-guides/install-git

https://github.blog/2015-06-08-how-to-undo-almost-anything-with-git/

[Dan Shiffman the Coding Train - Git and GitHub for Poets](https://www.youtube.com/playlist?list=PLRqwX-V7Uu6ZF9C0YMKuns9sLDzK6zoiV)

https://drjekyllthemes.github.io/all


### Other Repository Services

gitlab
bitbucket
sourceforge

### Interesting uses of Git

https://github.com/solarpunklab/solarpunk-lab


---

## Notes

Working Directory verses Local Repository?

Git doesn't need an internet connection, you can use it entirely locally on your computer.
Git is very lightweight, you should be able to use it easily on an old computer.

IMPORTANT - be careful what you put in a public git repository, including in the commit messages.  ie: no login credentials or other sensitive information.

Summary of 'Repository Settings'

Git compared with other collaboration and cloud tools like google-docs, dropbox, etherpad, etc...

### Ideas

Using branches to manage versions of your CV