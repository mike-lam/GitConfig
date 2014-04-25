============GIT BASH========
Michel@Michel-i5-PC ~/GitClone/GitSetup55
$ git clone http://rpi/git/GitSetup
Cloning into 'GitSetup'...
remote: Counting objects: 50, done.
remote: Compressing objects: 100% (45/45), done.
emote: Total 50 (delta 18), reused 0 (delta 0)
Unpacking objects: 100% (50/50), done.
Checking connectivity... done.

==============PUSH  ==================
command push 
select origin
===========PUSH use Tool Git Bash then ============
$ git push
warning: push.default is unset; its implicit value is changing in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the current behavior after the default changes, use:

  git config --global push.default matching

To squelch this message and adopt the new behavior now, use:

  git config --global push.default simple

When push.default is set to 'matching', git will push local branches
to the remote branches that already exist with the same name.

In Git 2.0, Git will default to the more conservative 'simple'
behavior, which only pushes the current branch to the corresponding
remote branch that 'git pull' uses to update the current branch.

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

Counting objects: 5, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 720 bytes | 0 bytes/s, done.
Total 3 (delta 1), reused 0 (delta 0)
To ssh://pi@rpi:/home/pi/git/GitSetup
   790be20..a74cdeb  master -> master


==========CLONE use Tool Git Bash then ============
$ git clone ssh://pi@rpi:/home/pi/git/GitSetup GitSetup
Cloning into 'GitSetup'...
remote: Counting objects: 38, done.
remote: Compressing objects: 100% (33/33), done.
Rremote: Total 38 (delta 10), reused 0 (delta 0)
Receiving objects: 100% (38/38), 89.32 KiB | 0 bytes/s, done.

Resolving deltas: 100% (10/10), done.
Checking connectivity... done.



================================

browser use http://rpi/gitweb

edit readme.txt
git commit -a
git push        now dont need origin and master since 1 push was done

did new file 
 git add .
 git commit
 git push origin master  this i needed I think the first time because 
                         original repo is bare, this works

did clone on pi
 git clone location

did on pi, bare as non bare does not allow push without a force of some kind
 git init --bare   

did on laptop
 install git
 install git extension
