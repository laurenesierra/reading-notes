# Git Tutorial: A Comprehensive Guide

- The __CVS system__ entails a single server storing all changes and file versions, which can be accessed by various clients.

- __DVCS__ allows clients to create mirrored repositories. Also, in the event of corruption of a central database’s hard disk — with the absence of backups — all work will be lost, except for any portions on local machines.

To prevent this type of catastrophic loss, a DVCS allows clients to create mirrored repositories. These data backups can be easily be placed on the server to replace any lost information.

##### What is Git?
- Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. 


#####  Files in Git can reside in three main states:

- Committed

Data is securely stored in a local database

- Modified

File has been changed but not committed to the database

- Staged

Flagged a file’s changed version to be committed in the next snapshot

##### Branching:
- Almost every type of Version Control System incorporates branching. By creating branches of a central repository, collaborators are able to work on a project simultaneously via multiple branches, without affecting this main repository.
- A Git branch is basically a movable pointer that always points to the most recent commit, or snapshot. Git uses the default local branch name “master”

##### There are two main categories of tags in Git: lightweight and annotated.

- Lightweight

A lightweight tag is a pointer to a particular commit – like a branch.

- Annotated

An annotated tag is stored in the Git database as a full object, containing a tagging message, tagger name and email, and tag date. Annotated Tags can also undergo signing and verification with GNU Privacy Guard (GPG). The best practice is to use annotated tags when possible, to allow for storage of valuable information and privacy safeguards.


##### Aliases 
- These allow users to navigate Git in an easier fashion. To save time and effort, one can create aliases for Git commands, which eliminates the need to type out an entire default Git command.


__Note:__ It’s always wise to check your repository before committing anything, to avoid accidentally committing certain file!


##### Distributed Workflow

- The centralized workflow
This entails the existence of one main hub, which can accept code. In this type of structure, many developers synchronize to this central repository, pushing and merging changes to it.


- Integration-Manager Workflow
This workflow structure involves multiple remote repositories. In this scenario, there is often one main project repository, and developers can have read access to others’ repositories and write access to their own. Those involved in the Integration-Manager Workflow create clones of the main project repository, push any changes to it, and ask the repository maintainer to pull in the pushed changes. The maintainer can add someone’s repository as a remote, test changes locally, merge them into their branch, and push back to their repository.

This workflow is commonly found with hub-centered resources, such as GitHub

GitHub’s collaboration workflow revolves around Pull Requests.

##### Here are the main steps of the GitHub collaboration workflow:

1. Create a topic branch from master.
1. Commit changes for the project.
1. Push the topic branch to the GitHub project.
1. Open a Pull Request.
1. Confer with team and perform additional commits, if applicable.
1. The project owner closes or merges the Pull Request.

https://blog.udemy.com/git-tutorial-a-comprehensive-guide/




[<===Markdown](../README.md)
