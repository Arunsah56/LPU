Microsoft Windows [Version 10.0.26200.7705]
(c) Microsoft Corporation. All rights reserved.

C:\Users\sahar>cd ..

C:\Users>cd sahar

C:\Users\sahar>cd desktop

C:\Users\sahar\Desktop>cd LPU

C:\Users\sahar\Desktop\LPU>mkdir DEMO-GIT

C:\Users\sahar\Desktop\LPU> code .

C:\Users\sahar\Desktop\LPU> cd DEMO-GIT

C:\Users\sahar\Desktop\LPU\DEMO-GIT>mkdir app.py

C:\Users\sahar\Desktop\LPU\DEMO-GIT>cd ..

C:\Users\sahar\Desktop\LPU> git status
fatal: not a git repository (or any of the parent directories): .git

C:\Users\sahar\Desktop\LPU>git init
Initialized empty Git repository in C:/Users/sahar/Desktop/LPU/.git/

C:\Users\sahar\Desktop\LPU>git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        app.py

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\sahar\Desktop\LPU>git add .

C:\Users\sahar\Desktop\LPU>git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   app.py


C:\Users\sahar\Desktop\LPU>git commit -m "first commit"
[master (root-commit) d2510bc] first commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 app.py

C:\Users\sahar\Desktop\LPU>git push origin main
error: src refspec main does not match any
error: failed to push some refs to 'origin'

C:\Users\sahar\Desktop\LPU>gh repo create
? What would you like to do? Push an existing local repository to github.com
? Path to local repository (.)

? Path to local repository .
? Repository name LPU
? Description s
? Visibility Public
✓ Created repository Arunsah56/LPU on github.com
? Add a remote? Yes
? What should the new remote be called? origin
? Would you like to push commits from the current branch to "origin"? Yes
Enumerating objects: 3, done.its from the current branch to "origin"? (Y/n) y
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 208 bytes | 69.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Arunsah56/LPU.git
 * [new branch]      HEAD -> master
branch 'master' set up to track 'origin/master'.
✓ Pushed commits to https://github.com/Arunsah56/LPU.git

C:\Users\sahar\Desktop\LPU>git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   app.py

no changes added to commit (use "git add" and/or "git commit -a")

C:\Users\sahar\Desktop\LPU>git add .

C:\Users\sahar\Desktop\LPU>git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   app.py


C:\Users\sahar\Desktop\LPU>git commit -m "DEMO-LPU modified"
[master 185d767] DEMO-LPU modified
 1 file changed, 1 insertion(+)

C:\Users\sahar\Desktop\LPU>git push origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/Arunsah56/LPU.git'

C:\Users\sahar\Desktop\LPU>git push origin master
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Writing objects: 100% (3/3), 271 bytes | 135.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Arunsah56/LPU.git
   d2510bc..185d767  master -> master

C:\Users\sahar\Desktop\LPU>git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   app.py

no changes added to commit (use "git add" and/or "git commit -a")

C:\Users\sahar\Desktop\LPU>git add .

C:\Users\sahar\Desktop\LPU>git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   app.py


C:\Users\sahar\Desktop\LPU>git commit -m "app is again modified"
[master 4734311] app is again modified
 1 file changed, 2 insertions(+), 1 deletion(-)

C:\Users\sahar\Desktop\LPU>git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/Arunsah56/LPU.git'

C:\Users\sahar\Desktop\LPU>git push -u origin master
fatal: unable to access 'https://github.com/Arunsah56/LPU.git/': schannel: SEC_E_UNTRUSTED_ROOT (0x80090325) - The certificate chain was issued by an authority that is not trusted.

C:\Users\sahar\Desktop\LPU>git push origin master
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 292 bytes | 292.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Arunsah56/LPU.git
   185d767..4734311  master -> master

C:\Users\sahar\Desktop\LPU>git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean

C:\Users\sahar\Desktop\LPU>git log
commit 47343110f2ebed84baa4fd19aa32ee91b643e415 (HEAD -> master, origin/master, origin/HEAD)
Author: Arun Sah <saharun2056@gmail.com>
Date:   Mon Feb 2 10:51:43 2026 +0530

    app is again modified

commit 185d767b9bc2c66c1d00c756d96ce3f48e062660
Author: Arun Sah <saharun2056@gmail.com>
Date:   Mon Feb 2 10:46:13 2026 +0530

    DEMO-LPU modified

commit d2510bc5aded24e9d0c13e6556238f7a8dd1ea14
Author: Arun Sah <saharun2056@gmail.com>
Date:   Mon Feb 2 10:36:27 2026 +0530

    first commit

C:\Users\sahar\Desktop\LPU>git branch test

C:\Users\sahar\Desktop\LPU>git branch dev

C:\Users\sahar\Desktop\LPU>git branch prod

C:\Users\sahar\Desktop\LPU>git branch
  dev
* master
  prod
  test

C:\Users\sahar\Desktop\LPU>git checkout dev
Switched to branch 'dev'

C:\Users\sahar\Desktop\LPU>git branch
* dev
  master
  prod
  test

C:\Users\sahar\Desktop\LPU>git checkout -b new
Switched to a new branch 'new'

C:\Users\sahar\Desktop\LPU>git branch
  dev
  master
* new
  prod
  test

C:\Users\sahar\Desktop\LPU>git branch -d new
error: cannot delete branch 'new' used by worktree at 'C:/Users/sahar/Desktop/LPU'

C:\Users\sahar\Desktop\LPU>git checkout dev
Switched to branch 'dev'

C:\Users\sahar\Desktop\LPU>git branch -d new
Deleted branch new (was 4734311).

C:\Users\sahar\Desktop\LPU>git branch
* dev
  master
  prod
  test

C:\Users\sahar\Desktop\LPU>