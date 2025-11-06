
### 7. Pull Changes Locally

1. **Pull the Latest Changes**
   - Run:
     ```bash
     git pull origin master
     ```
     
2. **Check how many branch you have localy**
  ###### List both remote-tracking branches and local branches
   -Run:
   ```sh
   git branch --all 
   ```

3.  **To create local branches for each remote branch**
   - Run:
     ```sh
      git checkout -b mybranch origin/mybranch
     ```

  or 
  ```sh
  for branch in $(git branch -r | grep -v '\->'); do
    git checkout --track $branch
  done
  ```

4. **Pull Latest Changes for All Branches**
   - Run:
  ```sh
  for branch in $(git branch | sed 's/* //'); do
    git checkout $branch
    git pull
  done
  ```

5. **Switch to you branch and modify a file then push it to your branch **
6. **Switch to you master branch**
7. **Merge your file**
   - Run:
     ```sh
     git merge mybranch
     ```
     
8.  **push to your main branch**
     ```sh
    git push origin master
    ```

9. **Delete you branch localy**
    ```sh
    git branch -d mybranch 
    ```

10. **Delete it from github**
    ```sh
    git push origin -D mybranch 
    ```
    