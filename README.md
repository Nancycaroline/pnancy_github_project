pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project
$ cd pnancy_github_project
bash: cd: pnancy_github_project: No such file or directory

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project
$ git init
Initialized empty Git repository in C:/Users/pnancy/pnancy_github_project/.git/

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (master)
$ git add .

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (master)  
$ git commit -m "Initial commits with text"
[master (root-commit) dce36ab] Initial commits with text
 Committer: Caroline P <pnancy@amazon.com>
Your name and email address were configured automatically based  
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:


After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 script1.txt
 create mode 100644 script2.txt

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (master)
$ git remote add origin https://github.com/Nancycaroline/pnancy_github_project.git

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (master)
$ git branch -M main

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (main)
$ git push -u origin main
info: please complete authentication in your browser...
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 14 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 234 bytes | 46.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Nancycaroline/pnancy_github_project.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (main)
$ git checkout -b branch1
Switched to a new branch 'branch1'

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (branch1)
$ git add
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
hint: Disable this message with "git config set advice.addEmptyPathspec false"

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (branch1)
$ git add .

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (branch1)
$ git commit -m "add script3.txt"
[branch1 be3f6ea] add script3.txt
 Committer: Caroline P <pnancy@amazon.com>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 script3.txt

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (branch1)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (main)
$ git merge script3.txt
merge: script3.txt - not something we can merge

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (main)
$ git merge branch1
Updating dce36ab..be3f6ea
Fast-forward
 script3.txt | 0
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 script3.txt

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (main)
$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 14 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 248 bytes | 248.00 KiB/s, done.
Total 2 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Nancycaroline/pnancy_github_project.git
   dce36ab..be3f6ea  main -> main

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (main)
$ git checkout -b rebase-branch
Switched to a new branch 'rebase-branch'

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (rebase-branch)
$ git add .

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (rebase-branch)
$ git commit -m "performing rebase"
[rebase-branch 98f1efd] performing rebase
 Committer: Caroline P <pnancy@amazon.com>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 script4.txt

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (rebase-branch)
$ git checkout rebase-branch
Already on 'rebase-branch'

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (rebase-branch)
$ git rebase main
Current branch rebase-branch is up to date.

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (rebase-branch)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (main)
$ git merge rebase-branch
Updating be3f6ea..98f1efd
Fast-forward
 script4.txt | 0
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 script4.txt

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (main)
$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 14 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 232 bytes | 25.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Nancycaroline/pnancy_github_project.git
   be3f6ea..98f1efd  main -> main

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (main)
$ git add .

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (main)
$ git commit -m "update the commits"
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (main)
$ git push
Everything up-to-date

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (main)
$ git config --global user.email "ssurendarnancy@gmail.com"

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (main)
$ git config --global user.name "Nancycaroline"

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (main)
$ git stash
No local changes to save

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (main)
$ git stash list

pnancy@HYD-7S0MH2Q9URJ MINGW64 ~/pnancy_github_project (main)
$ git stash apply
No stash entries found.

