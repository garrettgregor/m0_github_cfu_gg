**ALL** of the commands you know about git
- `git init` this command intializes a directory for git and keeps track of any changes within that folder
- `git add <filename>` this adds any filenames specified to the staging area so that they are ready to be committed
    - additionally, one can add all of the files within a given directory by using the command `git add .`; however, this is generally discouraged as it would be better to unwind to multiple different versions and doing the commit this way would lump multiple items together
- `git status` this shows me the status of changes within a given directory, and handily can even tell you whether you need to `add` or `commit`
- `git log` this will tell you what has been committed already
- `git diff` this will tell me a list of difference within the files that are already committed and what is in the staging area
- `git commit -m "MESSAGE"` this command commits what has been readied in the staging area; 
    - messages should be in the imperative present form and should make sense if you were to add "This commit will..." in front of it
## Pushing
- `git remote add origin [insert SSH key here]` after you have created a remote repo in [Github](github.com), this will set up a connection to ensure that you can push commits to the remote repo
- `git branch -M main` This sets the working branch for commits to be the main branch
- `git push -u origin main` This is the command you would use to push commits to the main branch
    - `git push` alternatively, if you had already set the working branch to main, then you could just use this command
- `git clone [insert SSH key here]` This would clone a remote repo to your local working directory - this can be useful is you have already forked a repo and would like to iterate on that particular branch/project
- `git remote remove origin` This command removes a remote connection
- `git remote -v` After using the above command, you could then use this command to check your remote connection to git