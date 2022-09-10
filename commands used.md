@j33l ➜ /workspaces/assign1 (master) $ git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
@j33l ➜ /workspaces/assign1 (master) $ git remote -v
origin  https://github.com/j33l/assign1 (fetch)
origin  https://github.com/j33l/assign1 (push)
upstream        https://github.com/Harry2482/assign1.git (fetch)
upstream        https://github.com/Harry2482/assign1.git (push)
@j33l ➜ /workspaces/assign1 (master) $ git branch
* master
@j33l ➜ /workspaces/assign1 (master) $ git checkout -b updatedNewBranch
Switched to a new branch 'updatedNewBranch'
@j33l ➜ /workspaces/assign1 (updatedNewBranch) $ git branch
  master
* updatedNewBranch
@j33l ➜ /workspaces/assign1 (updatedNewBranch) $ git status
On branch updatedNewBranch
nothing to commit, working tree clean
@j33l ➜ /workspaces/assign1 (updatedNewBranch) $ git add README.md temp.txt 
@j33l ➜ /workspaces/assign1 (updatedNewBranch) $ git status
On branch updatedNewBranch
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md
        new file:   temp.txt

@j33l ➜ /workspaces/assign1 (updatedNewBranch) $ git commmit -m "added new file and modified new file"
git: 'commmit' is not a git command. See 'git --help'.

The most similar command is
        commit
@j33l ➜ /workspaces/assign1 (updatedNewBranch) $ git commit -m "added new file and modified new file"
[updatedNewBranch e2ff94b] added new file and modified new file
 2 files changed, 15 insertions(+)
 create mode 100644 temp.txt
@j33l ➜ /workspaces/assign1 (updatedNewBranch) $ git log
commit e2ff94b415ba2f1f6f1be9315ad6459440a3aa20 (HEAD -> updatedNewBranch)
Author: Jeel <45571080+j33l@users.noreply.github.com>
Date:   Sat Sep 10 22:29:11 2022 +0000

    added new file and modified new file

commit 87907c5cbc7e26dd5f08ad87258f169e97d7e8fc (origin/master, origin/HEAD, master)
Author: Kyle Dewey <kyle.dewey@csun.edu>
Date:   Tue Sep 4 21:45:28 2018 -0700

    Added retrospective

commit 845975daaac324688b4cd69a73fb4461e5ce4252
Author: Kyle Dewey <kyle.dewey@csun.edu>
Date:   Tue Sep 4 21:43:01 2018 -0700

    Through step 8

commit 1eca980176ae5bc3528922210daf822451560fe8
Author: Kyle Dewey <kyle.dewey@csun.edu>
Date:   Tue Sep 4 21:27:30 2018 -0700

    showed example with the proper pull request settings

commit dd64fa0607950e47c7eeecf0c5631a37175eb437
Merge: 9a9505f 4504af5
Author: Kyle Dewey <kyle.dewey@csun.edu>
Date:   Tue Sep 4 21:21:28 2018 -0700

    Merge branch 'master' of github.com:CSUN-COMP587-F18/assign1

commit 9a9505fffbf29439c45470d6296e69885e9120ea
Author: Kyle Dewey <kyle.dewey@csun.edu>
Date:   Tue Sep 4 21:21:09 2018 -0700

    added picture showing where to click to start a pull request

@j33l ➜ /workspaces/assign1 (updatedNewBranch) $ git push - u origin updatedNewBranch
error: src refspec u does not match any
error: failed to push some refs to '-'
@j33l ➜ /workspaces/assign1 (updatedNewBranch) $ git push -u origin updatedNewBranch
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 532 bytes | 532.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'updatedNewBranch' on GitHub by visiting:
remote:      https://github.com/j33l/assign1/pull/new/updatedNewBranch
remote: 
To https://github.com/j33l/assign1
 * [new branch]      updatedNewBranch -> updatedNewBranch
branch 'updatedNewBranch' set up to track 'origin/updatedNewBranch'.
@j33l ➜ /workspaces/assign1 (updatedNewBranch) $ git push
Everything up-to-date
@j33l ➜ /workspaces/assign1 (updatedNewBranch) $ 
