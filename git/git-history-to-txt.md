```git
git --no-pager log --graph --all > git-history.txt
```

### 1. git --no-pager
--no-pager tells Git to bypass the pager and output the results as raw, plain text directly to the console. This is crucial here because we are redirecting the output to a file, and we don't want the pager's interactive controls messing up the text redirection.

### 2. log
The core Git command used to display the commit history of the repository.

### 3. --graph
This draws a text-based, ASCII art graph representing the branching and merging history of your repository on the left-hand side of the text. It shows you visually how branches split off and merged back together using characters like *, |, /, and \.

### 4. --all
By default, git log only shows the history of the branch you are currently on. Adding --all forces Git to show the commits of every single branch (local and remote), tags, and stashes in the entire repository history.