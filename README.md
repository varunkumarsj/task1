Git and Linux Commands — One-by-One List

Basic Git Commands

1. git --version — Checks whether Git is installed and displays its version.

2. git config --global user.name "Your Name" — Sets the name Git records in your commits.

3. git config --global user.email "you@example.com" — Sets the email address Git records in your commits.

4. git clone <repository-url> — Downloads a copy of an existing Git repository from GitHub or another remote server.

5. git diff — Shows changes made to tracked files that have not yet been staged.

6. git fetch origin — Downloads information about updates from the remote repository without merging them into your current branch.

7. git help — Displays help information about Git commands.
2. Check the Repository
8. git status — Shows the current branch, changed files, and whether changes are ready to commit.

9. git branch — Lists your local branches. The * symbol identifies the current branch.

10. git remote -v — Displays the remote repository URLs connected to your local project.
3. Add and Save Changes
11. git init — Creates a new Git repository in the current folder. Use it only when the folder is not already a repository.

12. git add README.md — Stages the README.md file for the next commit.

13. git add . — Stages changes in the current directory, including new, modified, and deleted files.

14. git commit -m "Your message" — Saves staged changes as a commit with a descriptive message.

15. git push origin main — Uploads local commits from the main branch to GitHub.

16. git pull origin main — Downloads and integrates changes from GitHub's main branch into your local main branch.
4. Branch Commands
17. git switch -c testing — Creates a new branch called testing and switches to it.

18. git switch main — Switches to the existing main branch.

19. git push -u origin testing — Pushes the testing branch to GitHub and sets up tracking between the local and remote branches.

20. GitHub Pull Request (PR) — Requests that changes from one branch be reviewed and merged into another branch.

21. git branch -d testing — Deletes the local testing branch after it has been merged.

22. git push origin --delete testing — Deletes the remote testing branch from GitHub.
5. Commit History Commands
23. git log --oneline — Displays the commit history, with each commit shown on one short line.

24. git log -3 --oneline — Displays only the three most recent commits.
6. Revert and Synchronize Changes
25. git revert 062ccf1 — Creates a new commit that reverses the changes made by commit 062ccf1. Replace this example ID with the actual commit ID.

26. Esc, then :wq, then Enter — Saves and closes the Vim editor when Git opens it for a commit message.

27. git pull --rebase origin main — Downloads remote changes and replays your local commits on top of the updated main branch. This can help when a push is rejected because the remote has newer commits.

28. git push origin main — Pushes your local commits to GitHub after the update or rebase succeeds.
7. .gitignore Commands
29. Set-Content .gitignore "*.log" — In Windows PowerShell, creates or replaces .gitignore with a rule to ignore files ending in .log.

30. Set-Content application.log "This is a sample log file" — Creates a sample file named application.log.

31. git check-ignore application.log — Checks whether Git is ignoring application.log.

32. git add .gitignore — Stages the .gitignore file.

33. git commit -m "Added gitignore to ignore log files" — Saves the .gitignore change as a commit.

34. git push origin main — Uploads the .gitignore commit to GitHub.

Note: .gitignore does not automatically stop tracking files that Git already tracks.
8. Check the Default Branch
35. git remote show origin — Displays information about the remote repository, including its default branch.

36. git branch — Lists local branches and shows which one you are currently using.

Your repository already uses main as its default branch, so you do not need to rename it.
9. Linux Commands
These commands are used in Linux terminals such as Ubuntu or WSL.

37. pwd — Displays the full path of the current directory.

38. mkdir devops_practice — Creates a folder named devops_practice.

39. cd devops_practice — Moves into the devops_practice folder.

40. touch file1.txt file2.txt file3.txt — Creates three empty files.

41. ls — Lists the files and folders in the current directory.

42. mv file1.txt renamed_file.txt — Renames file1.txt to renamed_file.txt.

43. rm file3.txt — Deletes file3.txt. Be careful because the file usually is not moved to the Trash.

44. cd .. — Moves up one level to the parent directory.
10. Common Git Terms
45. Repository — A project whose changes are tracked by Git.

46. Branch — A separate line of development or work.

47. Stage — Select changes to include in the next commit.

48. Commit — A saved snapshot of staged changes.

49. Remote — A repository stored elsewhere, such as on GitHub.

50. origin — The common name for the remote repository connected to your local project.

51. Push — Sends local commits to the remote repository.

52. Pull — Brings remote changes into your local branch.

53. Merge — Combines changes from one branch into another.

54. Revert — Creates a new commit to undo the changes from an earlier commit.

55. .gitignore — A file that tells Git which untracked files to ignore.
11. Final Check
56. git status — Checks whether there are uncommitted changes.

57. git log --oneline — Reviews your commit history.

If git status displays nothing to commit, working tree clean, your working directory has no uncommitted changes.