# GitHub Exercise: Building and Collaborating on a Project

## Objective

Learn the basics of GitHub by creating a repository, making changes to files, and collaborating with others.

## Prerequisites

- A GitHub account (sign up at [github.com](https://github.com) if you don't have one).
- Git installed on your computer (download from [git-scm.com](https://git-scm.com)).

## Instructions

### 1. Create a New Repository

1. **Log in to GitHub**
   - Go to [github.com](https://github.com) and log in with your credentials.

### 2. Clone Your Repository to Your Local Machine

1. **Copy the Repository URL**
   - Go to your repository page on GitHub.
   - Click the green “Code” button and copy the URL provided (HTTPS or SSH).

2. **Open Terminal/Command Prompt**
   - Navigate to the directory where you want to clone the repository.
   - Run the following command:
     ```bash
     git clone <repository-url>
     ```
     Replace `<repository-url>` with the URL you copied.

3. **Navigate into the Repository**
   - ```bash
     cd my1stRepO
     ```

### 3. Make Changes Locally

1. **Create a New File**
   - Run the following command:
     ```bash
     touch hello.txt
     ```
     (For Windows, use: `echo. > hello.txt`)

2. **Add Content to the File**
   - Open `hello.txt` in a text editor and add the following text: `Hello, GitHub!`
   - Save and close the file.

3. **Check the Status**
   - Run:
     ```bash
     git status
     ```

4. **Stage Your Changes**
   - Run:
     ```bash
     git add hello.txt
     ```

5. **Commit Your Changes**
   - Run:
     ```bash
     git commit -m "Add hello.txt with greeting message"
     ```

### 4. Push Your Changes to GitHub

1. **Push Your Changes**
   - Run:
     ```bash
     git push origin master
     ```
     
2. **Verify on GitHub**
   - Go back to your repository page on GitHub and refresh the page. You should see `hello.txt` listed.

### 5. Collaborate with Others

1. **Create a Branch**
   - Run
     ```sh
     git branch mybranch
     ```

   - or Run:
     ```bash
     git checkout -b mybranch
     ```

3. **Make Changes in the New Branch**
   - Create a new file:
     ```bash
     touch FileInMybranch.txt
     ```
   - Add content: Open `FileInMybranch.txt` and write "This is a File In My branch."

4. **Stage and Commit Your Changes**
   - Run:
     ```bash
     git add FileInMybranch.txt
     ```
   - Run:
     ```bash
     git commit -m "Bla Bla Bla"
     ```

5. **Push Your Branch to GitHub**
   - Run:
     ```bash
     git push origin mybranch
     ```

6. **Create a Pull Request**
   - Go to your repository page on GitHub.
   - Click the “Compare & pull request” button.
   - Add a title and description for your pull request.
   - Click “Create pull request.”

### 6. Merge the Pull Request

1. **Review the Pull Request**
   - On GitHub, review your pull request.
   - If everything looks good, click “Merge pull request” and then “Confirm merge.”

2. **Delete the Branch**
   - After merging, you can delete the branch by clicking “Delete branch” on the pull request page.

### 7. Pull Changes Locally

1. **Switch Back to Main Branch**
   - Run:
     ```bash
     git checkout master
     ```

2. **Pull the Latest Changes**
   - Run:
     ```bash
     git pull origin master
     ```

## Summary

- Created a repository on GitHub.
- Cloned it to your local machine.
- Made and committed changes, then pushed them back to GitHub.
- Created a new branch, made additional changes, and merged those changes via a pull request.

Feel free to repeat these steps with different files and changes to get more comfortable. Happy coding! 🚀