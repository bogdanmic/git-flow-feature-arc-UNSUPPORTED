git-flow-feature-arc
====================

This is the git-flow-feature file from <https://github.com/nvie/gitflow> with a few modifications to use "arc diff" and "arc amend" to open and close review requests.
All the credits for building git-flow belong to its original owner.

To use this file, rewrite the original file from <https://github.com/nvie/gitflow> named **git-flow-feature** with this one and install gitflow as usual.

**NOTE:** Use this file at your own risk. It is very likely that it will not be maintained with any bugfixes ore modifications that apprea in the future to the original file.


#### What is so special about this file?

Well first for it to work you need to have installed this <https://github.com/facebook/arcanist> installed.
This is part of a larger process that uses [phabricator](http://phabricator.org/) to do code review.

For more details on installing **Phabricator** please check their documentation <http://www.phabricator.com/docs/phabricator/article/Installation_Guide.html>

After you do that, this file allows you to:
 
 - create a code review request to the phabricator server
 			
 		git flow feature review   # it executes "arc diff develop"
 - close the review requests after they are accepted
 
 		git flow feature finish   # it executes "arc amend" at the beginning of the normal process
 		
 		
I hope this is clear enough. If not, ask and maybe i will listen :)

#### Works on
It works on mac and other linux based systems.
Don't know about widows though.