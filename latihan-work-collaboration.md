# Latihan work colaboration 
## Silahkan edit dibawah ini
student8@student8-PC MINGW32 ~
$ dir
AppData
Application\ Data
Brainmatics\ Modul
Contacts
Cookies
Desktop
Documents
Downloads
Favorites
Links
Local\ Settings
Music
My\ Documents
NTUSER.DAT
NTUSER.DAT{016888bd-6c6f-11de-8d1d-001e0bcde3ec}.TM.blf
NTUSER.DAT{016888bd-6c6f-11de-8d1d-001e0bcde3ec}.TMContainer00000000000000000001.regtrans-ms
NTUSER.DAT{016888bd-6c6f-11de-8d1d-001e0bcde3ec}.TMContainer00000000000000000002.regtrans-ms
NetHood
Pictures
PrintHood
Recent
Saved\ Games
Searches
SendTo
Start\ Menu
Templates
Videos
ntuser.dat.LOG1
ntuser.dat.LOG2
ntuser.ini

student8@student8-PC MINGW32 ~
$ cd d:
bash: cd: d:: No such file or directory

student8@student8-PC MINGW32 ~
$ cd documents

student8@student8-PC MINGW32 ~/documents
$ dir
Java\ EE\ Web\ Application  My\ Music     My\ Videos   software
Java\ SE                    My\ Pictures  desktop.ini

student8@student8-PC MINGW32 ~/documents
$ dir
Java\ EE\ Web\ Application  My\ Music     My\ Videos  desktop.ini
Java\ SE                    My\ Pictures  Training    software

student8@student8-PC MINGW32 ~/documents
$ dir
Java\ EE\ Web\ Application  My\ Music     My\ Videos  desktop.ini
Java\ SE                    My\ Pictures  Training    software

student8@student8-PC MINGW32 ~/documents
$ cd training

student8@student8-PC MINGW32 ~/documents/training
$ git
usage: git [--version] [--help] [-C <path>] [-c name=value]
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
   bisect     Find by binary search the change that introduced a bug
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
   rebase     Forward-port local commits to the updated upstream head
   tag        Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch      Download objects and refs from another repository
   pull       Fetch from and integrate with another repository or a local branch
   push       Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.

student8@student8-PC MINGW32 ~/documents/training
$ git config --global user.name "Jon Maryono"

student8@student8-PC MINGW32 ~/documents/training
$ git config --global user.name "jonriau"

student8@student8-PC MINGW32 ~/documents/training
$ git config --global user.email "jon.riau@gmail.com"

student8@student8-PC MINGW32 ~/documents/training
$ dir
Day\ 1

student8@student8-PC MINGW32 ~/documents/training
$ dir
Note.txt

student8@student8-PC MINGW32 ~/documents/training
$ git init ../documents/training
Initialized empty Git repository in C:/Users/student8/documents/documents/training/.git/

student8@student8-PC MINGW32 ~/documents/training
$ git init ../training
Initialized empty Git repository in C:/Users/student8/documents/training/.git/

student8@student8-PC MINGW32 ~/documents/training (master)
$ dir
Note.txt

student8@student8-PC MINGW32 ~/documents/training (master)
$ git add Note.txt

student8@student8-PC MINGW32 ~/documents/training (master)
$ git commit -m "Catatan Pelatihan"
[master (root-commit) f866c04] Catatan Pelatihan
 1 file changed, 1 insertion(+)
 create mode 100644 Note.txt

student8@student8-PC MINGW32 ~/documents/training (master)
$ git remote add origin https://github.com/jonriau/training-java.git

student8@student8-PC MINGW32 ~/documents/training (master)
$ gir push -u origin master
bash: gir: command not found

student8@student8-PC MINGW32 ~/documents/training (master)
$ git push -u origin master
Username for 'https://github.com': jonriau
Password for 'https://jonriau@github.com':
Counting objects: 3, done.
Writing objects: 100% (3/3), 223 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/jonriau/training-java.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.

student8@student8-PC MINGW32 ~/documents/training (master)
$ git push -u origin master
Username for 'https://github.com': jonriau
Password for 'https://jonriau@github.com':
Branch master set up to track remote branch master from origin.
Everything up-to-date

student8@student8-PC MINGW32 ~/documents/training (master)
$ git add Note.txt

student8@student8-PC MINGW32 ~/documents/training (master)
$ git commit -m "Catatan Git"
[master a0a2293] Catatan Git
 1 file changed, 14 insertions(+), 1 deletion(-)

student8@student8-PC MINGW32 ~/documents/training (master)
$ git remote add origin https://github.com/jonriau/training-java.git
fatal: remote origin already exists.

student8@student8-PC MINGW32 ~/documents/training (master)
$ git remote add origin https://github.com/jonriau/training-java.git
fatal: remote origin already exists.

student8@student8-PC MINGW32 ~/documents/training (master)
$ git push -u origin master
Username for 'https://github.com': jonriau
Password for 'https://jonriau@github.com':
Counting objects: 3, done.
Delta compression using up to 2 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 406 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/jonriau/training-java.git
   f866c04..a0a2293  master -> master
Branch master set up to track remote branch master from origin.

student8@student8-PC MINGW32 ~/documents/training (master)
$ cd ..

student8@student8-PC MINGW32 ~/documents
$ md Training_Brainmatics
bash: md: command not found

student8@student8-PC MINGW32 ~/documents
$ git clone https://github.com/jonriau/training-brainmatics-2015-1 /Training-Brainmatics
fatal: could not create work tree dir 'C:/Program Files (x86)/Git/Training-Brainmatics': Permission denied

student8@student8-PC MINGW32 ~/documents
$ git clone https://github.com/jonriau/training-brainmatics-2015-1 ./Training-Brainmatics
Cloning into './Training-Brainmatics'...
remote: Counting objects: 15, done.
remote: Compressing objects: 100% (11/11), done.
remote: Total 15 (delta 4), reused 13 (delta 2), pack-reused 0
Unpacking objects: 100% (15/15), done.
Checking connectivity... done.

student8@student8-PC MINGW32 ~/documents
$ git pull
fatal: Not a git repository (or any of the parent directories): .git

student8@student8-PC MINGW32 ~/documents
$ dir
Java\ EE\ Web\ Application  My\ Pictures  Training-brainmatics
Java\ SE                    My\ Videos    desktop.ini
My\ Music                   Training      software

student8@student8-PC MINGW32 ~/documents
$ cd Training

student8@student8-PC MINGW32 ~/documents/Training (master)
$ git pull
Already up-to-date.

student8@student8-PC MINGW32 ~/documents/Training (master)
$ git status
On branch master
Your branch is up-to-date with 'origin/master'.
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   Note.txt

no changes added to commit (use "git add" and/or "git commit -a")

student8@student8-PC MINGW32 ~/documents/Training (master)
$ git status Note.txt
On branch master
Your branch is up-to-date with 'origin/master'.
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   Note.txt

no changes added to commit (use "git add" and/or "git commit -a")

student8@student8-PC MINGW32 ~/documents/Training (master)
$ git status Note.txt
On branch master
Your branch is up-to-date with 'origin/master'.
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   Note.txt

no changes added to commit (use "git add" and/or "git commit -a")

student8@student8-PC MINGW32 ~/documents/Training (master)
$ git clone o-date.
fatal: repository 'o-date.' does not exist

student8@student8-PC MINGW32 ~/documents/Training (master)
$

student8@student8-PC MINGW32 ~/documents/Training (master)
$ cd ..

student8@student8-PC MINGW32 ~/documents
$ git clone https://github.com/ellozius/training-brainmatics-h1.git ./Training-elos
Cloning into './Training-elos'...
remote: Counting objects: 6, done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 6 (delta 0), reused 6 (delta 0), pack-reused 0
Unpacking objects: 100% (6/6), done.
Checking connectivity... done.

student8@student8-PC MINGW32 ~/documents
$ git clone https://github.com/ellozius/training-brainmatics-h1.git ./Training-elos
fatal: destination path './Training-elos' already exists and is not an empty directory.

student8@student8-PC MINGW32 ~/documents
$ git pull
fatal: Not a git repository (or any of the parent directories): .git

student8@student8-PC MINGW32 ~/documents
$ git clone https://github.com/ellozius/training-brainmatics-h1.git ./Training-elos
Cloning into './Training-elos'...
remote: Counting objects: 10, done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 10 (delta 1), reused 9 (delta 0), pack-reused 0
Unpacking objects: 100% (10/10), done.
Checking connectivity... done.

student8@student8-PC MINGW32 ~/documents
$ git remote add ^C

student8@student8-PC MINGW32 ~/documents
$ git remote training-elos https://github.com/ellozius/training-brainmatics-h1.git
fatal: Not a git repository (or any of the parent directories): .git

student8@student8-PC MINGW32 ~/documents
$ dir
Java\ EE\ Web\ Application  My\ Pictures  Training-brainmatics  software
Java\ SE                    My\ Videos    Training-elos
My\ Music                   Training      desktop.ini

student8@student8-PC MINGW32 ~/documents
$ git remote elos https://github.com/ellozius/training-brainmatics-h1.git       fatal: Not a git repository (or any of the parent directories): .git

student8@student8-PC MINGW32 ~/documents
$ git remote elos https://github.com/ellozius/training-brainmatics-h1.git
fatal: Not a git repository (or any of the parent directories): .git

student8@student8-PC MINGW32 ~/documents
$ dir
Java\ EE\ Web\ Application  My\ Pictures  Training-brainmatics  software
Java\ SE                    My\ Videos    Training-elos
My\ Music                   Training      desktop.ini

student8@student8-PC MINGW32 ~/documents
$ cd Training
Training/             Training-brainmatics/ Training-elos/

student8@student8-PC MINGW32 ~/documents
$ cd Training-elos

student8@student8-PC MINGW32 ~/documents/Training-elos (master)
$ git remote elos https://github.com/ellozius/training-brainmatics-h1.git
error: Unknown subcommand: elos
usage: git remote [-v | --verbose]
   or: git remote add [-t <branch>] [-m <master>] [-f] [--tags | --no-tags] [--mirror=<fetch|push>] <name> <url>
   or: git remote rename <old> <new>
   or: git remote remove <name>
   or: git remote set-head <name> (-a | --auto | -d | --delete | <branch>)
   or: git remote [-v | --verbose] show [-n] <name>
   or: git remote prune [-n | --dry-run] <name>
   or: git remote [-v | --verbose] update [-p | --prune] [(<group> | <remote>)...]
   or: git remote set-branches [--add] <name> <branch>...
   or: git remote set-url [--push] <name> <newurl> [<oldurl>]
   or: git remote set-url --add <name> <newurl>
   or: git remote set-url --delete <name> <url>

    -v, --verbose         be verbose; must be placed before a subcommand


student8@student8-PC MINGW32 ~/documents/Training-elos (master)
$ dir
latihan-work-collaboration.md  readme.md  version-control.md

student8@student8-PC MINGW32 ~/documents/Training-elos (master)
$ git add latihan-work-collaboration.md

student8@student8-PC MINGW32 ~/documents/Training-elos (master)
$ git commit -m "perubahan kedua"
[master 4147bbe] perubahan kedua
 1 file changed, 1 insertion(+)

student8@student8-PC MINGW32 ~/documents/Training-elos (master)
$ git remote add elos https://github.com/ellozius/training-brainmatics-h1.git

student8@student8-PC MINGW32 ~/documents/Training-elos (master)
$ git -u elos master
Unknown option: -u
usage: git [--version] [--help] [-C <path>] [-c name=value]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

student8@student8-PC MINGW32 ~/documents/Training-elos (master)
$ git push -u elos master
Username for 'https://github.com': jonriau
Password for 'https://u@github.com':
remote: Invalid username or password.
fatal: Authentication failed for 'https://github.com/ellozius/training-brainmatics-h1.git/'

student8@student8-PC MINGW32 ~/documents/Training-elos (master)
$ git push -u elos master
Username for 'https://github.com': jonriau
Password for 'https://jo@github.com':
remote: Invalid username or password.
fatal: Authentication failed for 'https://github.com/ellozius/training-brainmatics-h1.git/'

student8@student8-PC MINGW32 ~/documents/Training-elos (master)
$ git push -u elos master
Username for 'https://github.com': jonriau
Password for 'https://jo@github.com':
remote: Invalid username or password.
fatal: Authentication failed for 'https://github.com/ellozius/training-brainmatics-h1.git/'

student8@student8-PC MINGW32 ~/documents/Training-elos (master)
$ git push -u elos master
jUsername for 'https://github.com':jonriau
Password for 'https://jonriau@github.com':
Counting objects: 3, done.
Delta compression using up to 2 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 317 bytes | 0 bytes/s, done.
Total 3 (delta 1), reused 0 (delta 0)
To https://github.com/ellozius/training-brainmatics-h1.git
   c9b24be..4147bbe  master -> master
Branch master set up to track remote branch master from elos.

student8@student8-PC MINGW32 ~/documents/Training-elos (master)
$ ^C

student8@student8-PC MINGW32 ~/documents/Training-elos (master)
$

