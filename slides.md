1. # Git for Everybody - Slide Notes

2. ## What is Git, and what can you do with it?

3. Version Control
	- How can you record changes to files, while keeping previous versions for reference?
	- Knowing which is the correct or most current version is a common problem.

4. Version Control
	- Version control is a system for managing changes to files over time, similar to using track changes in a word processor.
	- In the case of Git, a hidden ".git" folder is added to the project folder, where the history of changes to the files in the folder is recorded.
	- This turns the project folder into a Git Repository or "Repo" for short.
	- This means you can always work in the same file, and use the version control tool to revert it to a previous or different version at any time.

5. Open Source collaboration is complex
	- In a software project any single line of code can potentially have broad consequences, so managing contributions from a large group of collaborators is very complex.
	- Version control tools are crucial to allow groups of developers to simultaneously work on multiple versions of the same software.
	- As an example, this data vizualisation by Jeff Palmer shows some of the history of contributions to the Git software, which had almost 2000 contributors as of November 2020.

6. Where did Git come from?
	- Originally created by Linus Torvalds, the creator of Linux, for version control in the development of the Linux kernel.
	- Git itself is an open source project, and the most popular distributed version control system.

7. Git is "Distributed Version Control"
	- This means that every person working on a project has a complete local copy of of the whole project, including its full history.
	- Normally these copies are synced via a central server, but could also be synchronized in a peer-to-peer way.

8. What is the difference between Git and Github?
	- Git is open source version control software that is installed locally, and can be used to create a repository anywhere on your computer.
	- GitHub is an online Git hosting service, owned by Microsoft, that makes it easy to share repositories and collaborate on them.

9. There are many other Git hosting platforms
	- Whilst GitHub is the most popular, there are many other platforms that each have their own features and models. These are just some examples.
	- Gitlab, Gitea nad Forgejo are free and open-source services, meaning they can also be self-hosted on your own server.
	- Radicle uses a peer-to-peer protocol that allows repositories to be shared across a network without the need for a central server.

10. Git is a language
	- Not a programming language, but a collection of terminology that specify all the different actions that are involved when managing versions of files in a project and sharing and collaborating on those versions with other people.
	- Understanding this terminology is most of the challenge of learning Git, and can initially be quite confusing.
	- Aside from being able to use Git, I would argue that learning this language can also help inform your project development process and communication with collaborators.

11. When and why should you use Git?
	- As a local repository:
		- If you are working on anything in code, you should absolutely consider using Git (This is what it was built for, after all).
		- Any kind of writing - creative writing, research, legal code, etc...
		- Managing assets/content used across different projects.
		- You could even use it on a single file, like an accounts spreadsheet or a diary journal, if you put it in its own folder.
		- Anything that will change and gain complexity over time, where recording changes it could be useful.
		- Archives - creating a data repository or collection of archival material.
	- As a published repository:
		- Documentation:
			- Background information, installation/usage/execution instructions, credits and references.
			- Information that might change as a project develops.
		- For collaborating with friends and strangers.
	    - Turning a project "open source" - publishing the development material behind a project such that somebody else can reproduce or continue developing it.
		- Communicating with your audience - Git hosting platforms usually include discussion tools that allow for interaction between people using/viewing a repository and the authors.
	- Tracking and metrics - measuring progress on a project and keeping a historical record.

12. How I tend to use Git
	- Usually I have a folder called "repo" or "main" inside a project folder, which I use as a git repository. Here I keep production files, a project description and documentation, along with any instructions needed for using/building/installing/presenting the project.
	- Outside this folder I will keep anything else related to the project, which I feel is not necessary or inapporopriate to include in the repository, which may be or will become public in future.
	- Whilst transparency and documenation is great, it is also important to have a private space where you can explore your ideas without potentially putting them on permanent record.

13. What types of files work well with Git, and what do not?
	- Any kind of text-based file will work well with Git - meaning any kind of file that is human readable in a text editor.
	- Other kinds of files are interperted by Git as "binary files", and these can sometimes lead to Git running much more slowly and greatly inflating the size of the repository.
		- The key here is to avoid any large binary files, such as large video and audio files, large PDFs, and heavy project files such as photoshop documents.
	- Some software, such as Ableton and Kdenlive, do not embed video and audio data into the project file itself, but will link to external files. In this case, you can put the project file inside the Git repository, while excluding the linked files, and maintain a fast and lightweight repository while tracking changes to the project.

14. What is the difference between a "binary file" and a "text file"?
	- Actually, deep down all files are stored as ones and zeros, but "text files" are those which are encoded in a way that can be rendered as human-legible text in a text editor.
	- When tracking changes in text files, Git can clearly show us which lines have been edited and where.
	- In the case of binary files, it is much harder for Git to show us what has changed, usually we can only compare the entire file with its previous version.

15. What is Markdown?
	- Plain text by itself has no formatting (headings, bold, italic, bullets, etc...), so markup languages are used to specify formatting in plain text that can then be rendered with formatting on a web page as HTML in a PDF, for example.
	- Markdown was designed so that the plain text itself is still easy to read without needing to render the formatted version.
	- Has become widely adopted and supported as a formatting syntax for authoring text in many contexts, such as blogging, note taking, or writing documentation.
	- Due to its ubiquity, writing in markdown means your content will be easy to apply to many different contexts, probably well into the future, while always remaining easy to read in its plain text form.
	- Markdown syntax is very simple - the one key point that can be confusing are line breaks:
		- 

16. ## How do you use Git?

17. `git init`

18. `git commit`

19. `git branch`

20. `git checkout`

21. `git checkout`

22. `git checkout`

23. `git merge`

24. `git remote`

25. `git push`

26. `git pull`

27. `git clone`

28. `git clone`

29. `fork`

30. `pull request`

31. ## Food to Fork

32. `git fetch`

33. `git merge`

34. ## Turn your recipie into a webpage