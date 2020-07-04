# SubtreeTest
 trying out Git subtrees for the first time

## To create a subtree:
  * jaydp@LAPTOP-A71RG4T1 MINGW64 ~/Documents/Github/SubtreeTest (master)
    $ git remote add SubtreeTest-UILayer https://github.com/jaydpather/SubtreeTest-UILayer.git
  * jaydp@LAPTOP-A71RG4T1 MINGW64 ~/Documents/Github/SubtreeTest (master)
    $ git subtree add --prefix=SubtreeTest-UILayer/ SubtreeTest-UILayer master
    * --prefix is the folder name. (make this match the subtree repo name, for simplicity)
