# SubtreeTest
 trying out Git subtrees for the first time

## To create a subtree:
  * jaydp@LAPTOP-A71RG4T1 MINGW64 ~/Documents/Github/SubtreeTest (master)
    $ git remote add SubtreeTest-UILayer https://github.com/jaydpather/SubtreeTest-UILayer.git
  * jaydp@LAPTOP-A71RG4T1 MINGW64 ~/Documents/Github/SubtreeTest (master)
    $ git subtree add --prefix=SubtreeTest-UILayer/ SubtreeTest-UILayer master
    * --prefix is the folder name. (make this match the subtree repo name, for simplicity)
    * --note: this command specifies which branch of the Subtree repo you want (master)
  * once this is done, you can check the git history to see which commit was used for each subtree.
    * it seems there is no way to directly view which branch was used. You have to open the commit

## To make changes to a subtree via the main project:
  * make changes in main project, commit and push
  * then do:
    * git subtree push --prefix=SubtreeTest-UILayer/ SubtreeTest-UILayer master
    * git subtree push --prefix=[dirName] [subtreeName (same name you used in git subtree add)] [branch]

## To import changes made to subtree project:
  * git subtree pull —-prefix=SubtreeTest-UILayer/ SubtreeTest-UILayer master
  * git subtree pull -—prefix=[dirName] [subtreeName (same name you used in git subtree add)] [branch]
  
