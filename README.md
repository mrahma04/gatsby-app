# gatsby-app

### A little note on Git

If you start your project locally and then create a remote repo on GitHub with a README.md file for example, then you must 'fetch' and 'merge' the remote copy to the local branch. This way both your local and remote branches are in sync before you can start to commit changes etc.

This can be done by using the single `git pull origin main` command where 'origin' is the name of your remote repo and 'main' is the name of the (remote) branch that includes the README.md file.

To update the newly named 'main' branch in GitHub, use `git push origin master:main`. Here 'master' refers to the local 'master' branch and 'main' is the (remote) branch to be updated. If you don't specify it this way ('master:main') then git will automatically create a 'master' (remote) branch in GitHub.

To avoid this whole master/main debacle, it is simpler to just rename the local branch to 'main' when starting the project using `git branch -m master main`.

Once everything is in sync you might need to delete the remote branch using `git push origin --delete master`.
