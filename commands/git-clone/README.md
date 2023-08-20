<h1>
     <img align="center" width="40px" src="https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png"></a>
    <span> Learning Git</span>
</h1>

Doc Link: https://git-scm.com/docs. 

## Clonning Tips
Doc Link: https://git-scm.com/docs/git-clone.

When you clone a repository, you get files and history from a remote repository to a new folder in the current directory that you're working on.

### Simple Clonning
Plain and simple clone repository to the current folder. This command will create a new folder called **learning-git/** at your pc.

``` bash
$ git clone https://github.com/suilan/learning-git.git
Cloning into 'learning-git'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
Receiving objects: 100% (3/3), done.
$ ls
learning-git

```

### Clonning repository with another name
Sometimes, when we clone an repository, we need to rename it.


``` bash
$ mkdir learning
$ cd learning
$ git clone https://github.com/suilan/learning-git.git git
Cloning into 'learning-git'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
Receiving objects: 100% (3/3), done.
$ ls 
git
```

### Clonning repository quietly
You can use *-q* or *--quietly* to hide progress. If there is an error, the terminal will show it.

``` bash
$ git clone -q https://github.com/suilan/learning-git.git git
$ ls 
git
```

### Clonning repository with progress messages
You can use *-v* or *--verbose* to see every step of the progress.

``` bash
git clone -v https://github.com/suilan/learning-git.git git
Cloning into 'git'...
POST git-upload-pack (175 bytes)
POST git-upload-pack (252 bytes)
remote: Enumerating objects: 8, done.
remote: Counting objects: 100% (8/8), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 8 (delta 0), reused 5 (delta 0), pack-reused 0
Receiving objects: 100% (8/8), done.
```


### Clonning specific branch from repository
When you clone a repository, the default branch is the "main". But sometimes, you want to start on a specific feature/branch. Why? Project is too big, different application, different release, etc.

``` bash
$ git clone -v https://github.com/suilan/learning-git.git git --branch=feat/git-clone
Cloning into 'git'...
POST git-upload-pack (412 bytes)
POST git-upload-pack (252 bytes)
remote: Enumerating objects: 26, done.
remote: Counting objects: 100% (26/26), done.
remote: Compressing objects: 100% (15/15), done.
remote: Total 26 (delta 3), reused 23 (delta 3), pack-reused 0
Receiving objects: 100% (26/26), 4.02 KiB | 4.02 MiB/s, done.
Resolving deltas: 100% (3/3), done.
$ ls
git
$ cd git
$ git status
On branch feat/git-clone
Your branch is up to date with 'origin/feat/git-clone'.

nothing to commit, working tree clean

```





