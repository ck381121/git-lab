\\******
\\ answer 1
\\******
ckuhlwei@odd13:~$ cd cs2400/
ckuhlwei@odd13:~/cs2400$ mkdir git-lab
ckuhlwei@odd13:~/cs2400$ cd git-lab
ckuhlwei@odd13:~/cs2400/git-lab$ touch README.md
ckuhlwei@odd13:~/cs2400/git-lab$ touch answers.md
ckuhlwei@odd13:~/cs2400/git-lab$ git --version
git version 2.17.1
ckuhlwei@odd13:~/cs2400/git-lab$ 



\\*****
\\ answer 2
\\*****

ckuhlwei@odd13:~/cs2400/git-lab$ git config --global user.name "Christian Kuhlwein"
ckuhlwei@odd13:~/cs2400/git-lab$ git config --global user.email "ck381121@ohio.edu"
ckuhlwei@odd13:~/cs2400/git-lab$ git config --list
user.name=Christian Kuhlwein
user.email=ck381121@ohio.edu
ckuhlwei@odd13:~/cs2400/git-lab$ 






\\******
\\ answer 3
\\******

ckuhlwei@odd13:~/cs2400/git-lab$ git add --help
ckuhlwei@odd13:~/cs2400/git-lab$ git --help
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone      Clone a repository into a new directory
   init       Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add        Add file contents to the index
   mv         Move or rename a file, a directory, or a symlink
   reset      Reset current HEAD to the specified state
   rm         Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect     Use binary search to find the commit that introduced a bug
   grep       Print lines matching a pattern
   log        Show commit logs
   show       Show various types of objects
   status     Show the working tree status

grow, mark and tweak your common history
   branch     List, create, or delete branches
   checkout   Switch branches or restore working tree files
   commit     Record changes to the repository
   diff       Show changes between commits, commit and working tree, etc
   merge      Join two or more development histories together
   rebase     Reapply commits on top of another base tip
   tag        Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch      Download objects and refs from another repository
   pull       Fetch from and integrate with another repository or a local branch
   push       Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.


\\********
\\ git --help brings up a bunch of different commands that you can use
\\********







\\*****
\\Answer 4
\\*****


Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   README.md





\\*****
\\Answer 5
\\***** 

ckuhlwei@odd13:~/cs2400/git-lab$ git status README.md 
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   README.md



ckuhlwei@odd13:~/cs2400/git-lab$ git status README.md 
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   README.md

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   README.md









\\******
\\ answer 6
\\******

ckuhlwei@odd13:~/cs2400/git-lab$ git add answers.md 
ckuhlwei@odd13:~/cs2400/git-lab$ git status answers.md 
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   answers.md

ckuhlwei@odd13:~/cs2400/git-lab$ 



\\******
\\ answer 7
\\******

ckuhlwei@odd13:~/cs2400/git-lab$ git commit -m "Initial commit"
[master (root-commit) ac40886] Initial commit
 3 files changed, 2 insertions(+)
 create mode 100644 README.md
 create mode 100644 answers.md
ckuhlwei@odd13:~/cs2400/git-lab$ git status README.md 
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")





\\******
\\answer 8
\\******

ckuhlwei@odd13:~/cs2400/git-lab$ git log
commit ac408865229b302899b9afd49ad2d06b9481ef97 (HEAD -> master)
Author: Christian Kuhlwein <ck381121@ohio.edu>
Date:   Tue Aug 31 16:48:09 2021 -0400



\\******
\\answer 9
\\******


Counting objects: 4, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 321 bytes | 160.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0)
To https://github.com/ck381121/git-lab.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
ckuhlwei@odd13:~/cs2400/git-lab$ git status main
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean


\\******
\\answer 10
\\******

the file does not change locally

\\*****
\\answer 11
\\******

the push doesn't go through because the remote contains stuff that the file does not have locally

\\*****
\\answer 12
\\*****

the file now matches the online repository after the command git pull was used


\\****
\\answer 13
\\****

ckuhlwei@odd13:~/cs2400$ ls -a
.  ..  file.out  git-lab  git-lab-2












