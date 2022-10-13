# Stop tracking a tracked file

You have a node_modules folder that you do not want to be tracked by git.
You committed node_modules folder and now you realize that you forgot to ignore it using a .gitignore file. You add the .gitignore file and list the node_modules folder in it then commit.

But still Git is tracking it(node_modules). This is because, once a file has been added and committed to Git database, Git will continue tracking changes to it.

So you want to stop Git from tracking the node_modules folder.

Just run:
   ``git rm -r  --cached node_modules``
