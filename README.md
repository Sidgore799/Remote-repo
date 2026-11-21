1. Create a directory - mkdir git_repo
2. Create empty git repo. in local --> git init (It just initialize an empty repo. & give ability to perform git cmds actions) 
3. Create a file - touch git.txt 
4. git status --> To check Untracked, staged & Tracked status of any content
5. git add . --> To move all content ".", from untracked to staging area
6. git commit -m "Added file" --> To move staged content to Tracked area
7. git config --global user.name github_username --> To configure local repo. with remote repo. (Pre-requisites) 
8. git config --global user.email github_email --> To configure local repo. with remote repo. (Pre-requisites) 
9. git remote -v --> If it prints nothing, No remote is configured
10. git remote add origin https_url_of_git_repo --> To add remote repo. so, we cane push changes from local repo. to remote repo. (But, It ask for credentials for every push)
11. git remote set-url origin https://PAT@github.com/username/repo_name (To avoid to enter credentials everytime we use this method - Best Practice)
12. git push origin master (To send changes to remote repo. from local repo.)
13. git checkout -b dev
14. git branch
15. git switch master / git checkout master
16. git switch dev --> create a file - touch file1.txt --> git add file1.txt --> git commit -m "Added file1.text" --> git push origin dev
17. git switch master --> git merge dev --> git push origin master
18. Create a file - file2.txt --> git add file2.txt --> git rm --cached file2.txt -->
19. echo "hello" > file2.txt --> git add file2.txt --> git commit -m "add file2" # file2.txt is now tracked --> echo "oops" >> file2.txt # you edit it
    --> git restore file2.txt # "oops" is gone, the file is back to "hello"
20. If file already have text as - Hi --> echo "hello" > file2.txt --> O/P is hello (it removes previous value and update new value as > it redirects new value)
21. If file already have text as - Hi --> echo "hello" >> file2.txt --> O/P is Hi hello (in next line, as >> it appends value)
22. git diff --> To check changes in added file or staged area & untracked area
    e.g. echo "sid gore" > file2.txt --> git add file2.txt --> git commit -m "add file2" --> echo "gore sid" >> file2.txt # you edit the file --> git diff file2.txt
    o/p --> diff --git a/sid.txt b/sid.txt
index cf514b4..2ce2681 100644
--- a/sid.txt
+++ b/sid.txt
@@ -1 +1,2 @@
sid gore
+gore sid
23. vim .gitignore --> If we don't want to add or commit any file then we will create this .gitignore file & add that filename in this file so, that specific file will not be added to a staging area from untracked area
24. git clone ssh-url --> To copy remote repo. to the local
25. Fork - Goto any diffrent accounts repo. on github & clicked on fork buttom then you will get that repos. copy in your account 
 
