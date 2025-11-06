# Git Configuration Exercise

### Objective
Configure Git on your local machine and prepare a Git repository for version control.

### Prerequisites
- Git installed on your system. If not, download and install it from [git-scm.com](https://git-scm.com/).

### Steps
#### 0. Open your terminal and CHECK your git config file 

  ```sh
    cat ~/.gitconfig
   ```

#### 1. Configure Global User Information 
1. Set your global username and email address.
###### These details will be used for commits:

    ```sh
    git config --global user.name "Your Name"
    git config --global user.email "your.email@example.com"
    ```

3. Verify your configuration by checking the settings:

    ```sh
    git config --global --list
    ```

#### 2. Configure Default Text Editor
1. Set the default text editor that Git will use for commit messages. For example, to use `nano`:
###### This is an OPTIONAL step , alternatively, you can use any other text editor you prefer.
.

    ```sh
    git config --global core.editor "nano"
    ```
 #### 3. Create a New Git Repository
1. Navigate to a directory where you want to create your new Git repository:

    ```sh
    mkdir my1stRepO
    cd my1stRepO
    ```

2. Initialize a new Git repository:

    ```sh
    git init
    ```

#### 4. Create a New File and Make Your First Commit
1. Create a new file named `README.md` and add some content to it:

    ```sh
    echo "# My New Repo" > README.md
    ```

2. Stage the new file for commit:

    ```sh
    git add README.md
    ```

3. Commit the changes with a message:

    ```sh
    git commit -m "Initial commit with README.md"
    ```

#### 5. Set Up a Remote Repository (Optional)
1. If you want to push your local repository to a remote server like GitHub, GitLab, or Bitbucket, create a new repository on the remote server (e.g., GitHub).

2. Add the remote repository URL:

    ```sh
    git remote add origin https://github.com/your-username/my1stRepO.git
    ```

3. Push your local commits to the remote repository:

    ```sh
    git push -u origin master
    ```

#### 6. Explore Additional Configurations (Optional)
1. Set up an alias for a common Git command to make it shorter. For example, create an alias for `git status`:

    ```sh
    git config --global alias.st status
    ```

   Now you can use `git st` instead of `git status`.

#### Practice and Test

###### 1. Make some changes to `README.md` (e.g., add more text).
###### 2. Stage and commit these changes.
###### 3. Check the status and log to see your commit history.
###### 4. Experiment with the aliases and configurations you’ve set up.