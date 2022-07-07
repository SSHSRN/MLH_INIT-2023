# GIT

Command prompt => predates Powershell.
    |=> came out first.
    |=> Powershell also hass support for UNIX commands.
        |=> For example, clear is a UNIX command and it works in Powershell 
            and not in command prompt.

To list all possible commands, use the " git help --all " command

Github vs Gitlab:
    GitLab is both a free and open-source self-hosting service (Community Edition) 
    and a closed-source service (Professional Edition) (Enterprise Edition). 

    On the other hand, GitHub is not open-source and offers free repositories and private 
    repositories, which are widely used to host open-source web projects, 
    may include a premium plan.

git init --bare => initialises a bare repository.
The --bare flag creates a repository that doesn’t have a working directory, 
making it impossible to edit files and commit changes in that repository. 
You would create a bare repository to git push and git pull from, but never directly commit 
to it. Central repositories should always be created as bare repositories because pushing 
branches to a non-bare repository has the potential to overwrite changes. 

Think of --bare as a way to mark a repository as a storage facility, as opposed to a 
development environment. This means that for virtually all Git workflows, the central 
repository is bare, and developers local repositories are non-bare.
In git bare repository, we cannot commit directory to the repository.

commit => takes the current changes and applies it to the master(main branch).

Readme.md file => for documentation.

.gitignore => ignore files (not upload selected files to github.)

clone vs fork:
    * clone => clones the repo (user gets the same version of the repo and can commit to it).
        |=> used by a team of developers.
    * fork => creates another version of the same repository.
        |=> used by developers(contributors) who want to add on to an open source project.

commit vs push:
    * Pushing comes after committing. 
    * Git commit records and tracks changes to the repository with each commit points to a tree object 
        that captures the state of the repository at that moment the commit was performed, all in one complete snapshot. 
        But commits saves the changes only to the local repository but not to the remote repository. 
    * Git push updates your committed changes and allows you to send them to the remote repository 
        where all of the developers can access them. 
        When you use the push command, it simply updates your changes to the upstream repository.