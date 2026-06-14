# Git Exercise

## Bundle 1

### Exercise 1

```bash
1. mkdir Git_Exercises # creates a folder for git exercise
2. git init # initializing a repository in Git_Exercises folder
3. touch file1.txt # creates a new file1.txt
4. touch file2.txt # creates a new file2.txt
5. nano file1.txt  # adds content to file1.txt
6. nano file2.txt  # adds content to file2.txt
7. git branch -M main # renames the branch name from master to main
8. git add . # stages changes in the current working directory
9. git commit -m "Added new files and content to it" # commits changes to local repository
10.  git remote add origin https://github.com/hirwaelysee/Git_Learning.git # connects to the remote repository
11. git push origin main # push changes to the remote repository
12. git branch dev # creates a new branch dev
13. git checkout dev # switches to dev branch
14. git branch test # creates a new branch test 
15. git checkout test # switch to test branch 
16. git checkout dev # switches back to dev branch
17. git branch -d test # deletes the test branch
```
### Exercise 2
```bash
1. touch home.html # created a new file
2. git add home.html # added the home.html
3. git stash #stashed the home.html after adding it.

4. touch about.html # created a new file
5. git add about.html # added the about.html
6. git stash #stashed the about.html after adding it.

7. touch team.html # created a new file
8. git add team.html # added the team.html
9. git stash #stashed the team.html after adding it.

10. git stash list #show the list of stashed changes
11. git stash pop stash@{1} #recovered the stash 1 because it containes about.html

12. git stash pop stash@{1} #recovered the stash 1 because it containes home.html

13. git commit -m "Added about and home page"
14. git stash pop #recovered the team.html
15. git reset --hard #removes the staged files. 
```
## Bundle 2

## Exercise 1

```
1. git checkout -b ft/bundle-2 
2. touch service.html #created service and added some content
3. git add service.html
4. git commit -m "Added service html page"
5. git push origin ft/bundle-2
6. then click on the link that will lead u to do a pull.
7. Do a pull request then add a reviewer
8. Wait for the response of the reviewer then merge the changes to the main.
```

## Exercise 2
```
1. git checkout main #switch to the main branch
2. git pull #Commit a pull in order for ur remote and local repository to be at the same page.
3. git checkout -b ft/service-redesign
4. Edit the service.html page.
5. git add service.html
6. git commit -m "Added some changes to the service.html"
7. git push origin ft/service-redesign
8. Go on github then click on the pull request part and click the pull request button and add a reviewer
9.git switch main
10. Edit the service.html
11. git add service.html
12. git commit -m "Added list of our services."
13. git push origin main
14. go back to the pr you will notice a merge conflict 
15. Then merge both of them 
16. git checkout ft/service-redesign 
17. git merge main
18. git diff
19. git add service.html
20. git commit
21. git push origin main
```
# Bundle3 

## Exercise 1
```
1. git checkout -b ft/team-page
2. touch team.html
3. git commit -m "Added content to the team page"
4. git push origin ft/team-page
5. Create the PR for the changes
6. git checkout main
7. git checkout -b ft/contact-page
8. git checkout ft/team-page
9. git log 
10. Check the the last commit and copy it
11. git checkout ft/contact-page
12. git cherry-pick (latest_commit)
13. touch contact.html
14. git add contact.html
15. git commit -m "Added a contact page"
16. git push origin ft/contact-page
17. Create a new PR for the contact page
18. git checkout -b ft/faq-page
19. touch faq.html # add some changes there
20. git add faq.html
21. git commit -m "Added faq page"
22. git push origin ft/faq-page
23. git revert (the commit id of team.html you copied before)
24. git push origin ft/faq-page
```
## Exercise 2
```
1. git checkout -b ft/home-page-redesign
2. git checkout main 
3. make some changes in one the files on main
4. git commit -m "Added some changes in the home page"
5. git push origin main
6. git switch ft/home-page-redesign
7. git rebase main # moves the commit and changes of the main branch on top of the commits of the ft/home-page-redesign
8. add some changes to the home.html
9. git add home.html
10. git commit -m "Added some changes on the home page"
11. git push origin ft/home-page-redesign
12. Create a PR
```
# Bundle4

## Exercise 1
```
1. git checkout main
2. git remote add git-copy https://github.com/hirwaelysee/Git-git-copy.git #having 2 remote repository
3. Make some changes to the home page
4. git add home.html
5. git commit -m "Added an emoji to the home page"
6. git push origin
7. git push git-copy

```
## Exercise 2
```
1. git checkout ft/footer
2. add some changes to the branch 
3. git add (file)
4. git commit -m "Added some changes"
5. add some changes to the branch 
6. git add (file)
7. git commit -m "Added some new changes" 
8. git push origin ft/footer
9. git checkout main
10. git checkout -b ft/squashing
11. git merge --squash ft/footer # this command is used imagine that you created many commits on a branch and merge them to another branch all those commits will come but with this command you get all the changes and get to commit them in a single line of commit.
12. git commit -m "footer changes squashing"
13. git push origin ft/squashing
14. then create a PR.
```
