---
title: "Branching & PR Instructions!"
section: "workflows"
category: "git-workflow"
topic: "branching-and-pr-instructions"
tags:
  - "git"
  - "github"
  - "pull-request"
  - "branching"
featured: false
source: "source/workflows/Branching & PR Instructions.docx"
audience: "participants"
content_type: "instructions"
status: "draft"
original_format: "docx"
related_sections: []
search_terms:
  - "branching instructions"
  - "pr instructions"
  - "pull request"
summary: ""
---

# Branching & PR Instructions!

If you are still learning this, take things slow and be sure to really understand each git command and what it is doing respective of your local environment and your GitHub remote repository.

For this exercise, you will need to navigate to your terminal. You should have a folder called "assignments". If you do not, please create a new folder called "assignments". This is where your projects will live.

```bash
User-Computer $ cd assignments
User-Computer $ pwd
/Users/user_name/Desktop/assignments
```

Inside that folder, you need to create a folder for your project. In this example, we called ours "recipe".

```bash
User-Computer $ mkdir recipe
User-Computer $ cd recipe
```

That folder should have a git installed. Run `git status`, to check if it is installed. If it is not install, you will see the following

```bash
User-Computer $ git status
fatal: not a git repository (or any of the parent directories): .git
```

If you have git installed, you will see the following

```bash
User-Computer $ git status
On branch main

No commits yet
```

To install git to your directory, make sure you are in the project directory that will house your project files.

```bash
User-Computer $ pwd
/Users/user_name/Desktop/assignments/recipe
User-Computer $ git init
Initialized empty Git repository in /Users/user_name/Desktop/assignments/recipe/.git/
```

Create a file in your directory with some code! See `index.html` being created below.

⚠️Note: Don't worry so far about the `DS_Store` file. You haven't learned about `.gitignore` (Pro tip: if you know about `.gitignore`, teach your pairs!)

Open your newly created folder on VisualStudio, create a new file, `index.html` and start working with the instructions for this week's project. Save your new code while still inside Visual Studio

In your terminal, use git to create a new branch.

```bash
User-Computer $ git checkout -b recipe-html-css
Switched to a new branch 'recipe-html-css'
```

Now that you have created a branch, you can add modified files. Do this AFTER you create a branch in git, not before. When in doubt, do `git status`.

Use git add and git commit to add and track files to your project repository.

```bash
User-Computer $ git add index.html
User-Computer $ git commit -m "first commit"
[recipe-html-css (root-commit) 4db3dd1] first commit
1 file changed, 9 insertions(+)
create mode 100644 recipe/index.html
```

Push your changes to your remote branch on GitHub

```bash
User-Computer $ git push origin recipe-html-css
```

If you are creating a new repo from GitHub, you may see instructions with similar commands (see below photos). We recommend for the sake of learning that you do not copy and paste these until you are familiar enough to recall the commands without looking. Please note your project name and be sure you are initializing git and pushing up the proper project's code.

```bash
User-Computer $ git remote add origin git@github.com:github_username/project_name.git
User-Computer $ git push <remote> <branch_name>
```

If you create a new repository that is NOT nested in your `techtonica_assignments` folder (see the next two screenshots).

If you're not sure if you have a remote git repository, run the command `git remote -v`. Your terminal will output your remote origin if you have initialized git. If you do not see anything output, you have not initialized git.

Once you push up your modified files to your remote repository, you should see the following

Click the green "Compare & pull request" button to begin creating your pull request.

Notice your PR link will look something like this in your URL

```text
https://github.com/your_username/project_title/pull/1
```

## Resources

- 🎦How to Create a Pull Request with Graduate Ruthie Irvin
- 📰The Ultimate GitHub Collaboration Guide
