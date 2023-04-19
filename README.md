
divyanshu@divyanshu-VirtualBox:~$ script long sem ass 5
Script started, file is long
divyanshu@divyanshu-VirtualBox:~$ ssh-keygen -t ed25519 -C bhardwajdivyancanada@gmail.com
Generating public/private ed25519 key pair.
Enter file in which to save the key (/home/divyanshu/.ssh/id_ed25519): 
/home/divyanshu/.ssh/id_ed25519 already exists.
Overwrite (y/n)? n
divyanshu@divyanshu-VirtualBox:~$ cat ~/.ssh/id_ed25519.pub
ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIBzWQpLECE0OxI4Pb74OWd7ynae1VWnVxw4428DqRzks bhardwajdivyancanada@gmail.com
divyanshu@divyanshu-VirtualBox:~$ ssh -T git@github.com
Hi divyanshubhardwaj2003! You've successfully authenticated, but GitHub does not provide shell access.
divyanshu@divyanshu-VirtualBox:~$ git config --global user.email bhardwajdivyancanada@gmail.com
divyanshu@divyanshu-VirtualBox:~$ git config --global user.name Divyanshu Bhardwaj
divyanshu@divyanshu-VirtualBox:~$ sudo mkdir /Utilities
[sudo] password for divyanshu: 
mkdir: cannot create directory ‘/Utilities’: File exists
divyanshu@divyanshu-VirtualBox:~$ git unit /Utilities
git: 'unit' is not a git command. See 'git --help'.

The most similar command is
	init
divyanshu@divyanshu-VirtualBox:~$ git init /Utilities
Reinitialized existing Git repository in /Utilities/.git/
divyanshu@divyanshu-VirtualBox:~$ cd /Utilities
divyanshu@divyanshu-VirtualBox:/Utilities$ git add *
fatal: detected dubious ownership in repository at '/Utilities'
To add an exception for this directory, call:

	git config --global --add safe.directory /Utilities
divyanshu@divyanshu-VirtualBox:/Utilities$ git add *commit
fatal: detected dubious ownership in repository at '/Utilities'
To add an exception for this directory, call:

	git config --global --add safe.directory /Utilities
divyanshu@divyanshu-VirtualBox:/Utilities$ ^C
divyanshu@divyanshu-VirtualBox:/Utilities$ 
GNU bash, version 4.4.20(1)-release (x86_64-pc-linux-gnu)
divyanshu@divyanshu-VirtualBox:/Utilities$ commit^C
divyanshu@divyanshu-VirtualBox:/Utilities$ 
divyanshu@divyanshu-VirtualBox:/Utilities$ 
divyanshu@divyanshu-VirtualBox:/Utilities$ 
divyanshu@divyanshu-VirtualBox:/Utilities$ 
divyanshu@divyanshu-VirtualBox:/Utilities$ 
divyanshu@divyanshu-VirtualBox:/Utilities$ ^C
divyanshu@divyanshu-VirtualBox:/Utilities$ git add *commit^C
divyanshu@divyanshu-VirtualBox:/Utilities$ 
divyanshu@divyanshu-VirtualBox:/Utilities$ git commit
fatal: detected dubious ownership in repository at '/Utilities'
To add an exception for this directory, call:

	git config --global --add safe.directory /Utilities
divyanshu@divyanshu-VirtualBox:/Utilities$ git commit^C
divyanshu@divyanshu-VirtualBox:/Utilities$ ^C
divyanshu@divyanshu-VirtualBox:/Utilities$ git commit
fatal: detected dubious ownership in repository at '/Utilities'
To add an exception for this directory, call:

	git config --global --add safe.directory /Utilities
divyanshu@divyanshu-VirtualBox:/Utilities$ cd
divyanshu@divyanshu-VirtualBox:~$ git branch yourfirstname
fatal: not a git repository (or any of the parent directories): .git
divyanshu@divyanshu-VirtualBox:~$ git branch Divyanshu Bhardwaj
fatal: not a git repository (or any of the parent directories): .git
divyanshu@divyanshu-VirtualBox:~$ ^C
divyanshu@divyanshu-VirtualBox:~$ git branch Divyanshu Bhardwaj
fatal: not a git repository (or any of the parent directories): .git
divyanshu@divyanshu-VirtualBox:~$ git init
Initialized empty Git repository in /home/divyanshu/.git/
divyanshu@divyanshu-VirtualBox:~$ cd /Utilities
divyanshu@divyanshu-VirtualBox:/Utilities$ git status
fatal: detected dubious ownership in repository at '/Utilities'
To add an exception for this directory, call:

	git config --global --add safe.directory /Utilities
divyanshu@divyanshu-VirtualBox:/Utilities$ git config --global --add safe.directory /Utilities
divyanshu@divyanshu-VirtualBox:/Utilities$ cd
divyanshu@divyanshu-VirtualBox:~$ git branch Divyanshu Bhardwaj
fatal: Not a valid object name: 'Bhardwaj'.
divyanshu@divyanshu-VirtualBox:~$ git branch Divyanshu 
fatal: Not a valid object name: 'master'.
divyanshu@divyanshu-VirtualBox:~$ git branch Divyanshu
fatal: Not a valid object name: 'master'.
divyanshu@divyanshu-VirtualBox:~$ git branch Divyanshu
fatal: Not a valid object name: 'master'.
divyanshu@divyanshu-VirtualBox:~$ git branch divyanshu
fatal: Not a valid object name: 'master'.
divyanshu@divyanshu-VirtualBox:~$ git switch Divyanshu
git: 'switch' is not a git command. See 'git --help'.
divyanshu@divyanshu-VirtualBox:~$ git --help
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone      Clone a repository into a new directory
   init       Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add        Add file contents to the index
   mv         Move or rename a file, a directory, or a symlink
   reset      Reset current HEAD to the specified state
   rm         Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect     Use binary search to find the commit that introduced a bug
   grep       Print lines matching a pattern
   log        Show commit logs
   show       Show various types of objects
   status     Show the working tree status

grow, mark and tweak your common history
   branch     List, create, or delete branches
   checkout   Switch branches or restore working tree files
   commit     Record changes to the repository
   diff       Show changes between commits, commit and working tree, etc
   merge      Join two or more development histories together
   rebase     Reapply commits on top of another base tip
   tag        Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch      Download objects and refs from another repository
   pull       Fetch from and integrate with another repository or a local branch
   push       Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
divyanshu@divyanshu-VirtualBox:~$ git switch Divyanshu
git: 'switch' is not a git command. See 'git --help'.
divyanshu@divyanshu-VirtualBox:~$ git checkout -b Divyanshu
Switched to a new branch 'Divyanshu'
divyanshu@divyanshu-VirtualBox:~$ git remote add origin git@github.com:JeffM
divyanshu@divyanshu-VirtualBox:~$ git@github.com:JeffMaitland/iot10125.git
bash: git@github.com:JeffMaitland/iot10125.git: No such file or directory
divyanshu@divyanshu-VirtualBox:~$ git remote show origin
Warning: Permanently added the ECDSA host key for IP address '140.82.112.4' to the list of known hosts.
ERROR: Repository not found.
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
divyanshu@divyanshu-VirtualBox:~$ git remote show origin
ERROR: Repository not found.
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
divyanshu@divyanshu-VirtualBox:~$ git remote add origin
usage: git remote add [<options>] <name> <url>

    -f, --fetch           fetch the remote branches
    --tags                import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --track <branch>  branch(es) to track
    -m, --master <branch>
                          master branch
    --mirror[=<push|fetch>]
                          set up remote as a mirror to push to or fetch from

divyanshu@divyanshu-VirtualBox:~$ git remote add origin  git@github.com:divyanshubhardwaj2003/Assignment-5.git
fatal: remote origin already exists.
divyanshu@divyanshu-VirtualBox:~$ git push -u origin main
error: src refspec main does not match any.
error: failed to push some refs to 'git@github.com:JeffM'
divyanshu@divyanshu-VirtualBox:~$ git push -u origin Divyanshu
error: src refspec Divyanshu does not match any.
error: failed to push some refs to 'git@github.com:JeffM'
divyanshu@divyanshu-VirtualBox:~$ git push -u origin Assignment-5
error: src refspec Assignment-5 does not match any.
error: failed to push some refs to 'git@github.com:JeffM'
divyanshu@divyanshu-VirtualBox:~$ git push -u origin Assignment-5
error: src refspec Assignment-5 does not match any.
error: failed to push some refs to 'git@github.com:JeffM'
divyanshu@divyanshu-VirtualBox:~$ git push -u origin divyanshubhardwaj2003
error: src refspec divyanshubhardwaj2003 does not match any.
error: failed to push some refs to 'git@github.com:JeffM'
divyanshu@divyanshu-VirtualBox:~$ git push -u origin Divyanshu
error: src refspec Divyanshu does not match any.
error: failed to push some refs to 'git@github.com:JeffM'
divyanshu@divyanshu-VirtualBox:~$ git push -u origin 
fatal: The current branch Divyanshu has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin Divyanshu

divyanshu@divyanshu-VirtualBox:~$ git push upstream origin Divyanshu
error: src refspec origin does not match any.
error: src refspec Divyanshu does not match any.
error: failed to push some refs to 'upstream'
divyanshu@divyanshu-VirtualBox:~$ git push --set-upstream origin Divyanshu
error: src refspec Divyanshu does not match any.
error: failed to push some refs to 'git@github.com:JeffM'
divyanshu@divyanshu-VirtualBox:~$ git push --set-upstream origin Divyanshu Bhardwaj
error: src refspec Divyanshu does not match any.
error: src refspec Bhardwaj does not match any.
error: failed to push some refs to 'git@github.com:JeffM'
divyanshu@divyanshu-VirtualBox:~$ -m origin
-m: command not found
divyanshu@divyanshu-VirtualBox:~$ git branch
divyanshu@divyanshu-VirtualBox:~$ git branch Divyanshu'
> 
> git branch Divyanshu'
fatal: 'Divyanshu

git branch Divyanshu' is not a valid branch name.
divyanshu@divyanshu-VirtualBox:~$ git checkout Divyanshu'
> git push -u origin Divyanshu'
error: pathspec 'Divyanshu
git push -u origin Divyanshu' did not match any file(s) known to git.
divyanshu@divyanshu-VirtualBox:~$ git branch nonu
fatal: Not a valid object name: 'Divyanshu'.
divyanshu@divyanshu-VirtualBox:~$ git branch 
divyanshu@divyanshu-VirtualBox:~$ git branch 
divyanshu@divyanshu-VirtualBox:~$ git branch nonu
fatal: Not a valid object name: 'Divyanshu'.
divyanshu@divyanshu-VirtualBox:~$ git branch Divyanhu
fatal: Not a valid object name: 'Divyanshu'.
divyanshu@divyanshu-VirtualBox:~$ git branch Divyanhu'
> git branch Divyanhu'
fatal: 'Divyanhu
git branch Divyanhu' is not a valid branch name.
divyanshu@divyanshu-VirtualBox:~$ git branch Divyanshu'
> git branch Divyanshu'
fatal: 'Divyanshu
git branch Divyanshu' is not a valid branch name.
divyanshu@divyanshu-VirtualBox:~$ git push --set-upstream origin Divyanshu'
> 
> git push --set-upstream origin Divyanshu'
fatal: remote part of refspec is not a valid name in Divyanshu

git push --set-upstream origin Divyanshu
divyanshu@divyanshu-VirtualBox:~$ git push --set-upstream origin Divyanshu'

git push --set-upstream origin Divyanshu'
fatal: remote part of refspec is not a valid name in Divyanshu

git push --set-upstream origin Divyanshu
divyanshu@divyanshu-VirtualBox:~$ git branch Divyanshu'
git remote add origin
> git@github.com:JeffMaitland/iot10125.git
> 
> git push --set-upstream origin Divyanshu'
                     
git push --set-upstream origin Divyanshu'
fatal: 'Divyanshu
git remote add origin
git@github.com:JeffMaitland/iot10125.git

git push --set-upstream origin Divyanshu' is not a valid branch name.
> 
> cd
> git remote -v
> git branch Divyanshu'
git branch Divyanshu'
fatal: remote part of refspec is not a valid name in Divyanshu

cd
git remote -v
git branch Divyanshu
> git branch nonu
> git branch divyanshu
> ^C
divyanshu@divyanshu-VirtualBox:~$ git push -u origin divyanshubhardwaj2003
error: src refspec divyanshubhardwaj2003 does not match any.
error: failed to push some refs to 'git@github.com:JeffM'
divyanshu@divyanshu-VirtualBox:~$ git push -u origin divyanshubhardwaj2003
error: src refspec divyanshubhardwaj2003 does not match any.
error: failed to push some refs to 'git@github.com:JeffM'
divyanshu@divyanshu-VirtualBox:~$ git checkout -b divyanshubahrdwaj2003
Switched to a new branch 'divyanshubahrdwaj2003'
divyanshu@divyanshu-VirtualBox:~$ git status
On branch divyanshubahrdwaj2003

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	.ICEauthority
	.assignment.4.swp
	.assignment4.swp
	.bash_history
	.bash_logout
	.bashrc
	.cache/
	.config/
	.doubt.txr.swp
	.gitconfig
	.gnupg/
	.local/
	.mozilla/
	.profile
	.selected_editor
	.ssh/
	.studentlist.sh.swp
	.sudo_as_admin_successful
	.swp
	.test.sh.swp
	.viminfo
	.while.loop.swo
	.while.loop.swp
	1.sh.save
	1.txt
	2.txt
	2.txt.save
	3.txt
	4.txt
	ASS 1 HTML
	ASS 3 P1 HTML
	ASS 3 P1 TEXT
	ASSIGNEMNT 5
	ASSIGNMENT 7
	ASSIGNMNT 6 CLASS
	CurrentDate
	Daysinamonth text
	Desktop/
	Downloads/
	FolderCreation.sh
	HardLink
	HeaderFile.h
	Internetblocker.sh
	My.files
	MyLinkedFile
	MyLinkedFilw
	MyProcesses
	Myfile
	Myprocesses
	Pictures/
	SEM LONG ASSS 4
	Security Test
	SourceFile1.c
	SourceFile2.c
	SymbolicLink
	Task1
	Task1.c
	Task3.c
	as4
	ass3
	ass5
	assignement 4 text
	assignment.2
	assignment.3
	assignment.4
	assignment4
	assignment6
	choice.
	daysinamonth
	hello-world
	hello-world.sh
	long
	names.ass
	scripts/
	semlongasspart2
	snap/
	studentlist.sh
	test.sh
	typescript
	while.
	while.loop

nothing added to commit but untracked files present (use "git add" to track)
divyanshu@divyanshu-VirtualBox:~$ git add file nonu
fatal: pathspec 'file' did not match any files
divyanshu@divyanshu-VirtualBox:~$ git add nonu
fatal: pathspec 'nonu' did not match any files
divyanshu@divyanshu-VirtualBox:~$ git ASSIGNMENT 5
git: 'ASSIGNMENT' is not a git command. See 'git --help'.
divyanshu@divyanshu-VirtualBox:~$ git add ASSIGNMENT 5
fatal: pathspec 'ASSIGNMENT' did not match any files
divyanshu@divyanshu-VirtualBox:~$ git add ASSIGNEMNT 5
fatal: pathspec 'ASSIGNEMNT' did not match any files
divyanshu@divyanshu-VirtualBox:~$ git  remote -v
origin	git@github.com:JeffM (fetch)
origin	git@github.com:JeffM (push)
divyanshu@divyanshu-VirtualBox:~$ git remote set-url origin https://github.com/divyanshubhardwaj2003
divyanshu@divyanshu-VirtualBox:~$ git  remote -v
origin	https://github.com/divyanshubhardwaj2003 (fetch)
origin	https://github.com/divyanshubhardwaj2003 (push)
divyanshu@divyanshu-VirtualBox:~$ git push -u origin divyanshubhardwaj2003
error: src refspec divyanshubhardwaj2003 does not match any.
error: failed to push some refs to 'https://github.com/divyanshubhardwaj2003'
divyanshu@divyanshu-VirtualBox:~$ git remote set-url origin divyanshubhardwaj2003/Assignment-5
divyanshu@divyanshu-VirtualBox:~$ git push -u origin divyanshubhardwaj2003
error: src refspec divyanshubhardwaj2003 does not match any.
error: failed to push some refs to 'divyanshubhardwaj2003/Assignment-5'
divyanshu@divyanshu-VirtualBox:~$ save

Command 'save' not found, but can be installed with:

sudo apt install atfs

divyanshu@divyanshu-VirtualBox:~$ script L ASS%
Script started, file is L
divyanshu@divyanshu-VirtualBox:~$ 

