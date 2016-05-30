# Using Git

This chapter will take you through first-time git setup steps, creating your first local repository, and the basics of using version control locally to record your own changes. So firstly, let's talk about what "version control" means, and specifically what git-style version control means.

## A brief guide to version control

Version Control Systems (VCS) are a way of recording changes to a file or files over time, with the ability to go back to a specific version of a file, or all the files in a project, at a later date. Changes to files, or patches, are stored within the project, or repository, and a file can be restored to a specific point in time by adding up the relevant patches.

Centralised VCS such as Subversion allow multiple people to work on a repository simultaneously. They store the repository and all its changes on a single server and each end-user or client simply downloads or checkes out the latest version or snapshot to use on their local computer. This means that the central server is a single point of failure. Losing that means losing the entire history of the project. The latest snapshot is still available on the client computers, but the record of all the changes has been lost.

Modern Distributed VCS, such as Git or Mercurial, get around this single point of failure by insisting that each end-user or client mirrors the entire repository onto their local computer. Each mirror, or clone, of the central repository can be used to restore the central one in the event of a failure and each client can have their own workflow for interacting with the central repository.

## Why Git

Git is not the only Distributed VCS tool out there, but it has become the most popular. It was always built with speed in mind, and the ability to efficiently handle large projects.

It is different to Subversion and other Centralised VCS because rather than storing each change as a patch to a specific file, it treats each change as a snapshot of the whole repository file structure. If a file in the structure hasn't changed, then Git simply stores a link back to the previous identical file.

**Old School CVCS:**

![Oldschool VCS](../images/oldschool_vcs.png "Images used under CC BY 3.0 from https://github.com/git/git-scm.com")

**New School DVCS:**

![Oldschool VCS](../images/newschool_vcs.png "Images used under CC BY 3.0 from https://github.com/git/git-scm.com")

Finally, nearly every Git operation is local, making it ideal for long train journeys!