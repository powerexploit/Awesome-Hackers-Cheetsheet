# **Git-CheetSheet For Hackers:**
Git is a version control system tool used by coders,devops engineers and programmers to manage the different version of projects or software. Git is now also used by hackers or Pentesters to develop their own Hacking,Automation and OSINT research tools.
> I always use git to develop new OSINT , pentesting and automation tools.
So here are some special and some sensitive git commands.

## **Installtion Of Git Vcs:**
Installation of git vcs is very simple I am explaining in following steps.
    
   **Windows:**
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

    **Linux\Ubuntu:**
      Git vcs is automatically installed in all linux flavour but in **ubuntu** you need to install git vcs in following ways.
      * Steps:
        * Open your terminal
        * Run sudo apt install git
        ```
        powerexploit@localhost:~$ sudo apt install git
        ```
        * Then Run git command
        ```
        powerexploit@localhost:~$ git
        usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
                   [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
                   [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
                   [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
                    <command> [<args>]
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
    root@kali:~$/Hack$ git config --global user.email "email_of_the_git_user"
    ```
   