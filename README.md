#CLI API For Extending Git Commands

####  Wouldn't you like to be able to make a new repository without ever having to leave terminal?
> - The answer is yes. [Read the syntax](#syntax)
> - If you said no. To bad. I made this for me.

---
To keep things private; make a file to which you will read secret data from in your home directory.
Type: ``$ cd ~ && touch .secrets``

Open the file and paste this in:

**Do not wrap anything in this file with single or double quotes**

First create a [Github Personal Access Token Here](https://github.com/settings/tokens/new): COPY THE CODE!

> email=YOUR-GITHUB-EMAIL

> githubApiAuthToken=Authorization: token PASTE-YOUR-TOKEN-HERE

> githubApiPlainAuthToken=PASTE-YOUR-TOKEN-HERE

> gitPassword=YOUR-GITHUB-PASSWORD

---
# Syntax
``$ git new <your repo name>``

**You can put spaces in your repo name.**
>Typing ``$ git new awesome new git repo``
Outputs ``$ git new awesome-new-git-repo``

---

- You can type ``$ git open`` to open the url of the repo you're currently in.
- You can type ``$ git open issue`` to open the "create new issue" url for the repo. 

---
**Open Pull Request**
> ``$ git open pull``
    This will create a pull request for the current branch you're on (Compare Branch)
    for mergining into Master Branch (Base Branch). It's always best to call this basic
    function from the branch you're working on to merge into master.
    
 > ``$ git open pull <new-branch>``
    This will create a pull request for the current branch you're on (Compare Branch)
    for mergining into <new-branch> (Base Branch).

> ``$ git open pull <branch-one> <branch-two>``
    This will create a pull request for <branch-two> (Compare Branch)
    to merge into <branch-one> (Base Branch). You can call this function from any branch.

> ``$ git open pull <branch-one> <branch-one>``
    This will create a pull request to merge into its self.



## Will be working on creating more API features. 
