# Git Branch Setup

This document describes the process of setting up three branches (`main`, `dev`, `test`) for a Git repository after forking and cloning a public repository.

## Step-by-Step Guide

### 1. Fork and Clone a Public Repository

1. **Fork a Repository**
   - Go to [GitHub](https://github.com) and find a public repository you'd like to fork.
   - Click the "Fork" button at the top right of the repository page to create a copy of the repository under your GitHub account.

2. **Clone the Forked Repository**
    ```sh
    git clone https://github.com/your-username/your-forked-repo.git
    ```
    - *Description*: Clones your forked repository from GitHub to your local machine.

3. **Navigate to the Repository Directory**
    ```sh
    cd your-forked-repo
    ```
    - *Description*: Changes the current directory to the cloned repository directory.

### 2. Create Branches (`main`, `dev`, `test`)

4. **Check Current Branch**
    ```sh
    git branch
    ```
    - *Description*: Lists all branches in the repository and shows the current branch.

5. **Create `main` Branch**
    ```sh
    git checkout -b main
    ```
    - *Description*: Creates and switches to a new branch named `main`.

6. **Push `main` Branch to Remote**
    ```sh
    git push -u origin main
    ```
    - *Description*: Pushes the `main` branch to the remote repository and sets the upstream.

7. **Create `dev` Branch from `main`**
    ```sh
    git checkout -b dev main
    ```
    - *Description*: Creates and switches to a new branch named `dev` from `main`.

8. **Push `dev` Branch to Remote**
    ```sh
    git push -u origin dev
    ```
    - *Description*: Pushes the `dev` branch to the remote repository and sets the upstream.

9. **Create `test` Branch from `dev`**
    ```sh
    git checkout -b test dev
    ```
    - *Description*: Creates and switches to a new branch named `test` from `dev`.

10. **Push `test` Branch to Remote**
    ```sh
    git push -u origin test
    ```
    


    
    - *Description*: Pushes the `test` branch to the remote repository and sets the upstream.
