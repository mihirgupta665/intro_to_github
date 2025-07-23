
📘 Git Cheat Sheet – with Explanations

 🛠️ Setup


git config --global user.name "[firstname lastname]"      # <!-- Set your name globally for Git commits -->
git config --global user.email "[valid-email]"            # <!-- Set your email globally for Git commits -->
git config --global color.ui auto                         # <!-- Enable colored output for easier reading -->



📁 Setup & Init

git init                                                  # <!-- Initialize an existing directory as a Git repository -->
git clone [url]                                           # <!-- Clone a remote Git repository to your local machine -->

📌 Stage & Snapshot

git status                                                # <!-- Show modified and staged files -->
git add [file]                                            # <!-- Stage changes to a specific file -->
git reset [file]                                          # <!-- Unstage a file but keep its changes -->
git diff                                                  # <!-- Show changes that are not staged -->
git diff --staged                                         # <!-- Show staged changes not yet committed -->
git commit -m "[descriptive message]"                     # <!-- Commit staged changes with a message -->


🌿 Branch & Merge


git branch                                                # <!-- List all local branches -->
git branch [branch-name]                                  # <!-- Create a new branch -->
git checkout [branch-name]                                # <!-- Switch to the specified branch -->
git merge [branch]                                        # <!-- Merge the specified branch into the current branch -->
git log                                                   # <!-- View commit history of the current branch -->

🌐 Share & Update

git remote add [alias] [url]                              # <!-- Add a remote repository URL with an alias -->
git fetch [alias]                                         # <!-- Download branches and updates from the remote -->
git merge [alias]/[branch]                                # <!-- Merge a remote branch into your local branch -->
git push [alias] [branch]                                 # <!-- Push your commits to a remote repository -->
git pull                                                  # <!-- Fetch and merge updates from the remote repository -->

📁 Tracking Path Changes

git rm [file]                                             # <!-- Remove file from working directory and stage deletion -->
git mv [existing-path] [new-path]                         # <!-- Rename or move a file and stage the change -->
git log --stat -M                                         # <!-- Show commit logs and track moved files -->

🧺 Temporary Commits (Stashing)

git stash                                                 # <!-- Save current modified/staged changes temporarily -->
git stash list                                            # <!-- List all saved stashes -->
git stash pop                                             # <!-- Reapply most recently stashed changes and remove them from stash -->
git stash drop                                            # <!-- Discard the most recent stash -->

🕘 Rewrite History

git rebase [branch]                                       # <!-- Reapply commits from the current branch on top of the given branch -->
git reset --hard [commit]                                 # <!-- Reset to a specific commit and discard all changes -->

🔍 Inspect & Compare

git log                                                   # <!-- Show full commit history -->
git log branchB..branchA                                  # <!-- Show commits in branchA but not in branchB -->
git log --follow [file]                                   # <!-- Show history of changes to a file (even through renames) -->
git diff branchB...branchA                                # <!-- Show differences in branchA not present in branchB -->
git show [SHA]                                            # <!-- Show detailed information about a specific commit or object -->

🚫 Ignoring Patterns

git config --global core.excludesfile [file]              # <!-- Set global ignore patterns -->

Example .gitignore contents:

logs/
*.notes
pattern*/ 

<!-- These patterns will prevent specified files or directories from being staged or committed -->
