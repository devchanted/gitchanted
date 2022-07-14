# Merging in git

Merging is the opposite of branching. Merging combines two seperate points 

Example:

1. Create a repo in github
    ```
    github.com > Repository > Create Repo merge
    ```
2. Clone repo to youe local 
    ```
    git clone <repo-url>
    ```
3. Navigate to your repo
    ```
    cd merge
    ```
4. Create a file
    ```
    touch file1.txt
    ```
5. Modify the file1.txt
    ```
    echo A > file1.txt
    ```
6. Add file to staging area
    ```
    git add file1.txt
    ```
7. Commit file 
    ```
    git commit -am 'A'
    ```
Repeat steps 5 -7 couple of times with newer data 

8. Create a new brach 
    ```
    git brach feature
    ```
9. Checkout new branch 
    ```
    git checkout feature
    ```
10. Modify the file1.txt
    ```
    echo D > file1.txt
    ```
11. Add file to staging area
    ```
    git add file1.txt
    ```
12. Commit file 
    ```
    git commit -am 'D'
    ```
Now that changes are seperate in both branches , lets try merging the changes in 'feature' branch to master branch

13. merge feature to master
    ```
    git checkout master
    ```
    ```
    git merge feature
    ```
    