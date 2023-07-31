1. create your own folder
    ```
    mkdir aa
    cd aa
    ```

    verify that the current folder is **not** tracked by Git:
    ```
    git status
    ```

2. create a new SAS program file
    ```
    echo "proc options; run;" > ./pgm/sas-git.sas
    ```

3. initialize a new repo by using the **git init** command
    ```
    git init --initial-branch==main
    ```

    This command creates a new git repository skeleton in a subdirectory named '.git' under the current directory. This meas that you're now able to start using other git commands in the current directory.

4. git configuration
    ```
    git config --list --show-origin | grep user
    ```
    or use this command in windows to check whether you set your name and email of github:

    ```
    git config --list --show-origin | findstr user
    ```

5. optional: set your basic identification configuration settings
    ```
    git config --global user.name "First-name Last-name"
    git config --global user.email emailAddress@provider
    ```
6. stage your project files with the **git add** command
    ```
    git add .
    git status
    ```

7. commit the files, we can use whether commit message (comment) we want
    ```
    git commit -m 'initial commit'
    ```

8. edit files, we can just use the ">>" to append something to the existing file's content
    ```
    echo "/* adding just a comment to the code */" >> ./pgm/sas-git.sas
    ```

9. stage and commit the files with this shortcut (-am means stage all and commit together)
    ```
    git commit -am "added a comment"
    ```