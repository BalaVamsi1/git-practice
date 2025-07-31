hp@bala-vamsi123-lanke MINGW64 ~
$ cd Desktop/edureka/GIT/sample-project/

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project
$ ls -l
total 8
drwxr-xr-x 1 hp 197121    0 Jul 31 14:12 css/
drwxr-xr-x 1 hp 197121    0 Jul 31 14:12 fonts/
drwxr-xr-x 1 hp 197121    0 Jul 31 14:12 img/
-rw-r--r-- 1 hp 197121 2866 Jul 31 14:12 index.html

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project
$ git init
Initialized empty Git repository in C:/Users/hp/Desktop/edureka/GIT/sample-project/.git/

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (main)
$ ls -l
total 8
drwxr-xr-x 1 hp 197121    0 Jul 31 14:12 css/
drwxr-xr-x 1 hp 197121    0 Jul 31 14:12 fonts/
drwxr-xr-x 1 hp 197121    0 Jul 31 14:12 img/
-rw-r--r-- 1 hp 197121 2866 Jul 31 14:12 index.html

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (main)
$ git config --global user.name "Mike"

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (main)
$ git config --global user.email "mike@aperturetech.com"

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (main)
$ git add .
warning: in the working copy of 'css/site.css', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'index.html', LF will be replaced by CRLF the next time Git touches it

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (main)
$ git commit -m ""intital commit"
> ^C

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (main)
$ git branch new-features
fatal: not a valid object name: 'main'

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (main)
$ ^C

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (main)
$ git log
fatal: your current branch 'main' does not have any commits yet

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (main)
$ git add .

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (main)
$ git commit -m 'first commit'
[main (root-commit) 9b37f13] first commit
 9 files changed, 198 insertions(+)
 create mode 100644 css/site.css
 create mode 100644 fonts/segoeuil.ttf
 create mode 100644 img/cloneWhite.svg
 create mode 100644 img/deployWhite.svg
 create mode 100644 img/lightbulbWhite.svg
 create mode 100644 img/stackWhite.svg
 create mode 100644 img/successCloudNew.svg
 create mode 100644 img/tweetThis.svg
 create mode 100644 index.html

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (main)
$ git branch new-feature

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (main)
$ git checkout new-feature
Switched to branch 'new-feature'

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (new-feature)
$ echo "<!-- New feature added by Mike -->" >> index.html
bash: !-: event not found

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (new-feature)
$ ls -l
total 8
drwxr-xr-x 1 hp 197121    0 Jul 31 14:12 css/
drwxr-xr-x 1 hp 197121    0 Jul 31 14:12 fonts/
drwxr-xr-x 1 hp 197121    0 Jul 31 14:12 img/
-rw-r--r-- 1 hp 197121 2866 Jul 31 14:12 index.html

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (new-feature)
$ vim index.html

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (new-feature)
$ git add index.html
warning: in the working copy of 'index.html', LF will be replaced by CRLF the next time Git touches it

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (new-feature)
$ git commit -m 'new code changes in index.html'
[new-feature 5c655d7] new code changes in index.html
 1 file changed, 2 insertions(+), 2 deletions(-)

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (new-feature)
$ git checkout main
Switched to branch 'main'

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (main)
$ git merge new-feature
Updating 9b37f13..5c655d7
Fast-forward
 index.html | 4 ++--
 1 file changed, 2 insertions(+), 2 deletions(-)

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (main)
$ git remote add origin https://github.com/BalaVamsi1/git-practice.git

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (main)
$ git push -u origin main
Enumerating objects: 17, done.
Counting objects: 100% (17/17), done.
Delta compression using up to 4 threads
Compressing objects: 100% (15/15), done.
Writing objects: 100% (17/17), 460.66 KiB | 6.06 MiB/s, done.
Total 17 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), done.
To https://github.com/BalaVamsi1/git-practice.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (main)
$ git push origin new-feature
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'new-feature' on GitHub by visiting:
remote:      https://github.com/BalaVamsi1/git-practice/pull/new/new-feature
remote:
To https://github.com/BalaVamsi1/git-practice.git
 * [new branch]      new-feature -> new-feature

hp@bala-vamsi123-lanke MINGW64 ~/Desktop/edureka/GIT/sample-project (main)
$
