# GIT NOTES

groupadd dev            # add new group

useradd -G devs -d /home/gituser -m -s /bin/bash gituser             # add new user

git status                 the files you changed appear

git add .                  changed files are added

git status                 changed and added files appear

git commit -m 'Initial commit'           changed changes are committed

git push                  integrates changes into the project

git clone gituser@git.server.com:project.git            The Clone operation creates an instance of the remote repository.

git pull               synchronize his local repository with the remote one

git stash               takes your modified tracked files, stages changes, and saves them on a stack of unfinished changes that you can reapply at any time.

git rm string_operations       remove this file from the repository

