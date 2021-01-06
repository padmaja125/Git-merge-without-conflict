$ vi index.html

$ git add ,
fatal: pathspec ',' did not match any files

$ git add .
warning: LF will be replaced by CRLF in index.html.
The file will have its original line endings in your working directory

$ git commit -m 'updated index.html'
[master ca0b813] updated index.html
 1 file changed, 1 insertion(+)

$ git branch my-new-feature

$ git checkout my-new-feature
Switched to branch 'my-new-feature'

$ vi about-us.html

$ git add .

$ git commit -m 'commit in branch'
[my-new-feature 41457b4] commit in branch
 1 file changed, 1 insertion(+)

$ git checkout master
Switched to branch 'master'
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

$ git merge my-new-feature
Updating ca0b813..41457b4
Fast-forward
 about-us.html | 1 +
 1 file changed, 1 insertion(+)

$ git push
Logon failed, use ctrl+c to cancel basic credential prompt.
Username for 'https://github.com': padmaja125
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 704 bytes | 176.00 KiB/s, done.
Total 6 (delta 0), reused 0 (delta 0)
To https://github.com/padmaja125/exercise-8.git
   94d7e3e..41457b4  master -> master
