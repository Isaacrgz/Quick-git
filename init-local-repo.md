# Case

## Init local repo
In terminal

1) Place it the main folder
2) Init the repo with a custom branch name
   
   ```
   git init --initial-branch=<branch-name>
   ```
3) Add the remote repo previously created and worked with

   ```
   git remote add origin <https://github.com/account/repo-name.git>
   ```
4) Fetch the remote repo

   ```
   git fetch origin
   ```
5) Pull from remote repo
  
    ```
    git pull origin main --allow-unrelated-histories
    ```
6) Create gitingnore file

    ```
    echo. > .gitignore
    ```
7) Add `target/`

> [!WARNING]
> This step is only necessary if you want to prevent pushing post-compiled files.

## Push to remote repo

8) Stage the files
  
    ```
    git add .
    ```
9) Make the commit

    ```
    git commit -m "<message>"
    ```
10) Push to remote branch
    ```
    git push origin main
    ```
> [!NOTE]
> First, the ref `origin` and the remote branch `main` must be added.
