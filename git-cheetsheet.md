# **Git-CheetSheet For Hackers:**
Git is a version control system tool used by coders,devops engineers and programmers to manage the different version of projects or software. Git is now also used by hackers or Pentesters to develop their own Hacking,Automation and OSINT research tools.
> I always use git to develop new OSINT , pentesting and automation tools.
So here are some special and some sensitive git commands.

## **Installtion Of Git Vcs:**
Installation of git vcs is very simple I am explaining in following steps.
    
### **Windows:**
* Steps:
  * Download git vcs from https://git-scm.com/downloads
  * Install git.exe in windows
  * Open Your cmd and run git command
       ```
       C:\windows\system32> git
       usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
                  [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
                  [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
                  [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
                  <command> [<args>]
	```

### **Linux\Ubuntu:**
Git vcs is automatically installed in all linux flavour but in **ubuntu** you need to install git vcs in following ways.
* Steps:
  * Open your terminal
  * Run sudo apt install git

        ```
        root@localhost:~$ sudo apt install git
        ```

  * Then Run git command

        ```
        root@localhost:~$ git
        ```


# **Git Cheet Commands:**

  * Git command To create Repository:
    ```
    root@kali:~$ git init Hack
    ```
    > Hack is a name of Repository

  * Git command To Add file in Repository:
    ```
    root@kali:~/Hack$ git add exploit.py
    ```
    > exploit.py is the name of your file.
 
  * Git command To Commit in repo:
   
    **What is git commit?**
    Git commit is used to save changes to your local Hack repository.
    ```
    root@kali:~/Hack$ git commit -m "Added exploit file"
    ```
    > -m option is used to add messages in your save changes.
    
    ```
    root@kali:~/Hack$ git commit -a -m "Your message"   
    ```
   > -a option to commit all the files.

 * Git command To configure the commit in repo:
   
    ```
    root@kali:~/Hack$ git config --global user.name  "name_of_git_user"
    ```
    
    ```
    root@kali:~/Hack$ git config --global user.email "email_of_the_git_user"
    ```
 * Git command To check The Status Of Your repo:
   * What is git status?
     * Git status command displays the state of the working directory and the staging area. It lets you see which changes have been staged, which haven't, and which files aren't being tracked by Git.


    ```
    root@kali:~/Hack$ git status
    ```

 * Git push/pull command:
   * What is git push?
     * git push command is used to push the code in your github repository.
   * What is git pull?
     * git pull command is a Git command used to update the local version of a repository from a remote

    ```
    root@kali:~/Hack$ git push origin master
    root@kali:~/Hack$ git pull
    ```
##### **What is master is above command?**
Its a very neccessary concept for beginners in git and open source , **master** is a branch in your code repositry. **Branch** is just like a container of your current commits.

     ```
     root@kali:~/Hack$ # Git command to check your current branch
     root@kali:~/Hack$ git branch
     ```
 * Git command to check status of your repo:
    ```
    root@kali:~/Hack$ git status
    ```


