# Our first md-File

Markdown is a simple text file
fprmat to write structured text

## Second Level Headline

- Types of Headlines
  - Two Hashes do a secon d level headline
  - Three Hashes: guess what
- 

### Third Level
We do not know what to write here...

samistan@MacBook-Pro-von-Sami first_git % git --version
git version 2.56.0
samistan@MacBook-Pro-von-Sami first_git % git init
Reinitialized existing Git repository in /Users/samistan/Desktop/Schule/2026_27/SYPP/first_git/.git/
samistan@MacBook-Pro-von-Sami first_git % git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)
samistan@MacBook-Pro-von-Sami first_git % ls -a      
.               ..              .git            README.md
samistan@MacBook-Pro-von-Sami first_git % git add README.md 
samistan@MacBook-Pro-von-Sami first_git % git status 
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md

samistan@MacBook-Pro-von-Sami first_git % git commit -m "Added README.md"
[main (root-commit) 602b3c8] Added README.md
 Committer: Sami Stan <samistan@MacBook-Pro-von-Sami.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 13 insertions(+)
 create mode 100644 README.md
samistan@MacBook-Pro-von-Sami first_git % git config --global --edit
samistan@MacBook-Pro-von-Sami first_git % git config --global user.name "Stan Sami"
samistan@MacBook-Pro-von-Sami first_git % git config --global user.email "samiroland1@yahoo.com"
samistan@MacBook-Pro-von-Sami first_git % git commit -m "Added README.md"                       
On branch main
nothing to commit, working tree clean
samistan@MacBook-Pro-von-Sami first_git % git status                                            
On branch main
nothing to commit, working tree clean
samistan@MacBook-Pro-von-Sami first_git % ls
README.md
samistan@MacBook-Pro-von-Sami first_git % git log
commit 602b3c86efdb3627c9f9d9651b6f0e9eecdb3454 (HEAD -> main)
Author: Sami Stan <samistan@MacBook-Pro-von-Sami.local>
Date:   Thu Oct 15 18:20:16 2026 +0200

    Added README.md
samistan@MacBook-Pro-von-Sami first_git % ls -a 
.               ..              .git            README.md
samistan@MacBook-Pro-von-Sami first_git % echo README.md 
README.md
samistan@MacBook-Pro-von-Sami first_git % nano README.md 
samistan@MacBook-Pro-von-Sami first_git % touch another.md
samistan@MacBook-Pro-von-Sami first_git % echo "Das ist irgend ein Text" > another.md 
samistan@MacBook-Pro-von-Sami first_git % git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        another.md

no changes added to commit (use "git add" and/or "git commit -a")
samistan@MacBook-Pro-von-Sami first_git % touch anotheranother.md
samistan@MacBook-Pro-von-Sami first_git % echo "#lksajdhfjahs" > anotheranother.md 
samistan@MacBook-Pro-von-Sami first_git % git add README.md 
samistan@MacBook-Pro-von-Sami first_git % git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        another.md
        anotheranother.md

samistan@MacBook-Pro-von-Sami first_git % git comit -m "Some inportant Text"
git: 'comit' is not a git command. See 'git --help'.

The most similar command is
        commit
samistan@MacBook-Pro-von-Sami first_git % git commit -m "Some inportant Text"
[main 3935746] Some inportant Text
 1 file changed, 2 insertions(+), 1 deletion(-)
samistan@MacBook-Pro-von-Sami first_git % git log
commit 3935746d2a81224b7a316643d8271ef88db9972e (HEAD -> main)
Author: Stan Sami <samiroland1@yahoo.com>
Date:   Thu Oct 15 18:34:54 2026 +0200

    Some inportant Text

commit 602b3c86efdb3627c9f9d9651b6f0e9eecdb3454
Author: Sami Stan <samistan@MacBook-Pro-von-Sami.local>
Date:   Thu Oct 15 18:20:16 2026 +0200

    Added README.md
samistan@MacBook-Pro-von-Sami first_git % man git
samistan@MacBook-Pro-von-Sami first_git % git stauts
git: 'stauts' is not a git command. See 'git --help'.

The most similar command is
        status
samistan@MacBook-Pro-von-Sami first_git % git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        another.md
        anotheranother.md

nothing added to commit but untracked files present (use "git add" to track)
samistan@MacBook-Pro-von-Sami first_git % git add . 
samistan@MacBook-Pro-von-Sami first_git % git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   another.md
        new file:   anotheranother.md

samistan@MacBook-Pro-von-Sami first_git % git commit -m "Addes new files"
[main 050830c] Addes new files
 2 files changed, 2 insertions(+)
 create mode 100644 another.md
 create mode 100644 anotheranother.md
samistan@MacBook-Pro-von-Sami first_git % git status
On branch main
nothing to commit, working tree clean
samistan@MacBook-Pro-von-Sami first_git % git log
commit 050830c3eef51d5e38cd4c5a3260e3e2f0f4044d (HEAD -> main)
Author: Stan Sami <samiroland1@yahoo.com>
Date:   Thu Oct 15 18:41:06 2026 +0200

    Addes new files

commit 3935746d2a81224b7a316643d8271ef88db9972e
Author: Stan Sami <samiroland1@yahoo.com>
Date:   Thu Oct 15 18:34:54 2026 +0200

    Some inportant Text

commit 602b3c86efdb3627c9f9d9651b6f0e9eecdb3454
Author: Sami Stan <samistan@MacBook-Pro-von-Sami.local>
Date:   Thu Oct 15 18:20:16 2026 +0200

    Added README.md
samistan@MacBook-Pro-von-Sami first_git % 