

commit 73e3718e95f521683d9bbca0c6882415641b733f
:
commit 1df068fb1f88fe6c1e017356cc70d6b0f1778dd3 (HEAD -> assignment, origin/branch2, branch2)
Author: srinu <srinurd81@gmail.com>
Date:   Wed Dec 13 22:28:15 2023 +0530

    'changes_done_two'

commit f0876c80eac011429f9226a4132a0c4ce2ea9ba2 (origin/assignment)
Author: srinu <srinurd81@gmail.com>
Date:   Wed Dec 13 22:23:10 2023 +0530

    'second_file_added'

commit 73e3718e95f521683d9bbca0c6882415641b733f
Author: srinu <srinurd81@gmail.com>
Date:   Wed Dec 13 22:18:03 2023 +0530

    'removed_two'

commit 30d8fd41cb73637fe227952f2542708c649e0419
Author: srinu <srinurd81@gmail.com>
Date:   Wed Dec 13 22:15:41 2023 +0530

    'added'
PS C:\Users\srinu\Desktop\food> git status
On branch assignment
Your branch is up to date with 'origin/assignment'.

nothing to commit, working tree clean
PS C:\Users\srinu\Desktop\food> git checkout -b master
Switched to a new branch 'master'
PS C:\Users\srinu\Desktop\food> git add third.html
PS C:\Users\srinu\Desktop\food> git commit -m 'third_Added'
[master 5e69632] third_Added
 1 file changed, 1 insertion(+)
 create mode 100644 third.html
PS C:\Users\srinu\Desktop\food> git push
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\srinu\Desktop\food> git restore
fatal: you must specify path(s) to restore
PS C:\Users\srinu\Desktop\food> git checkout assignment
Switched to branch 'assignment'
Your branch is up to date with 'origin/assignment'.
PS C:\Users\srinu\Desktop\food> git add third.html
fatal: pathspec 'third.html' did not match any files
PS C:\Users\srinu\Desktop\food> git add third.html
fatal: pathspec 'third.html' did not match any files
PS C:\Users\srinu\Desktop\food> git add .
PS C:\Users\srinu\Desktop\food> git commit -m 'changed_file2'
[assignment b2f0ac1] changed_file2
 1 file changed, 1 insertion(+), 1 deletion(-)
PS C:\Users\srinu\Desktop\food> git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 297 bytes | 297.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/srinu123-commits/frontend_assignment.git
   6b46568..b2f0ac1  assignment -> assignment
PS C:\Users\srinu\Desktop\food> git status   
On branch assignment
Your branch is up to date with 'origin/assignment'.

nothing to commit, working tree clean
PS C:\Users\srinu\Desktop\food> git checkout branch2
Switched to branch 'branch2'
Your branch is up to date with 'origin/branch2'.
PS C:\Users\srinu\Desktop\food> git two.html
git: 'two.html' is not a git command. See 'git --help'.
PS C:\Users\srinu\Desktop\food> git add two.html
PS C:\Users\srinu\Desktop\food> git commit -m 'file2_changed_on_branch2'
[branch2 15c5f3c] file2_changed_on_branch2
 1 file changed, 1 insertion(+), 1 deletion(-)
PS C:\Users\srinu\Desktop\food> git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 332 bytes | 332.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/srinu123-commits/frontend_assignment.git
   57b7de7..15c5f3c  branch2 -> branch2
PS C:\Users\srinu\Desktop\food> git checkout master
Switched to branch 'master'
PS C:\Users\srinu\Desktop\food> git merge assignment
Merge made by the 'ort' strategy.
 two.html | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)
PS C:\Users\srinu\Desktop\food> git merge branch2
Auto-merging two.html
CONFLICT (content): Merge conflict in two.html
Automatic merge failed; fix conflicts and then commit the result.
PS C:\Users\srinu\Desktop\food> git merge branch2
fatal: You have not concluded your merge (MERGE_HEAD exists).
Please, commit your changes before you merge.
PS C:\Users\srinu\Desktop\food> git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   two.html

PS C:\Users\srinu\Desktop\food> git log
commit 6e9a13399b40fe1f804192cbf85527c04ab03083 (HEAD -> master, origin/master)
Merge: 42ecd53 15c5f3c
Author: srinu <srinurd81@gmail.com>
Date:   Wed Dec 13 22:55:05 2023 +0530

    Merge branch 'branch2'

commit 42ecd539d5d425e28e702f9ecbc10fd3c631b4cb
Merge: 5e69632 b2f0ac1
Author: srinu <srinurd81@gmail.com>
Date:   Wed Dec 13 22:52:35 2023 +0530

    Merge branch 'assignment'

commit 15c5f3c548b94d63bdcefce2525c682d3963af4d (origin/branch2, branch2)
Author: srinu <srinurd81@gmail.com>
Date:   Wed Dec 13 22:52:16 2023 +0530

    file2_changed_on_branch2

commit b2f0ac1fd86db68c76d5b0d74348a44b0b997547 (origin/assignment, assignment)
Author: srinu <srinurd81@gmail.com>
Date:   Wed Dec 13 22:50:53 2023 +0530

    changed_file2

commit 5e6963286b5ab5ec52d76d785d9caf067adf29cb
Author: srinu <srinurd81@gmail.com>
Date:   Wed Dec 13 22:48:59 2023 +0530

    third_Added

commit 57b7de7450dd4e81f58475161d460524460ffaf2
Author: srinu <srinurd81@gmail.com>
Date:   Wed Dec 13 22:40:59 2023 +0530

    test branch2

commit 6b46568f89a7b3a7379d8fd03fb6f1ead0473ece
Author: srinu <srinurd81@gmail.com>
Date:   Wed Dec 13 22:39:57 2023 +0530

    testing

commit 613ee16d6c5301d8bab3f54ec14f05b46f96704c
Author: srinu <140204901+srinu123-commits@users.noreply.github.com>
Date:   Wed Dec 13 22:35:09 2023 +0530

    Update README.md

commit 6cc5df4e7a6a390427a184bbf43ac1b09a41edb3
Author: srinu <140204901+srinu123-commits@users.noreply.github.com>
Date:   Wed Dec 13 22:34:17 2023 +0530

    Create README.md

commit 5369272e7f4a9694c7bfb1dc7847c50e84985b3b
Merge: f0876c8 1df068f
Author: srinu <140204901+srinu123-commits@users.noreply.github.com>
Date:   Wed Dec 13 22:32:25 2023 +0530

    Merge pull request #1 from srinu123-commits/branch2

    'changes_done_two'

commit 1df068fb1f88fe6c1e017356cc70d6b0f1778dd3
Author: srinu <srinurd81@gmail.com>
Date:   Wed Dec 13 22:28:15 2023 +0530

    'changes_done_two'

commit f0876c80eac011429f9226a4132a0c4ce2ea9ba2
Author: srinu <srinurd81@gmail.com>
Date:   Wed Dec 13 22:23:10 2023 +0530

    'second_file_added'

commit 73e3718e95f521683d9bbca0c6882415641b733f
Author: srinu <srinurd81@gmail.com>
Date:   Wed Dec 13 22:18:03 2023 +0530

    'removed_two'

commit 30d8fd41cb73637fe227952f2542708c649e0419
Author: srinu <srinurd81@gmail.com>
Date:   Wed Dec 13 22:15:41 2023 +0530

    'added'
