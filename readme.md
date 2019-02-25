#Intro
This experimental repository is getting documented during the work flow using [gitflow](https://danielkummer.github.io/git-flow-cheatsheet/ "git-flow are a set of git extensions to provide high-level repository operations for Vincent Driessen's branching model.")  git-flow branching style.

To get more familiar this  [GitFlow Examples](https://gitversion.readthedocs.io/en/latest/git-branching-strategies/gitflow-examples/ "These examples are using the default configuration with GitVersion. Which is continuous deployment mode for develop and continuous delivery mode for all other branches.") can help.

#####Initializing Project with `git flow init` command:  
 
    λ git flow init
    Initialized empty Git repository in C:/Cmder/docs/merdocs/.git/
    No branches exist yet. Base branches must be created now.
    Branch name for production releases: [master]
    Branch name for "next release" development: [develop]
    
    How to name your supporting branch prefixes?
    Feature branches? [feature/]
    Bugfix branches? [bugfix/]
    Release branches? [release/]
    Hotfix branches? [hotfix/]
    Support branches? [support/]
    Version tag prefix? []
    Hooks and filters directory? [C:/Cmder/docs/merdocs/.git/hooks]  

######Add remote to this repository

    λ git remote add origin https://github.com/user/documenting-guide.git

######Commit changes
     λ git add . && git commit -m "first commit, no branching yet"
    [develop a87a11b] first commit, no branching yet
     1 file changed, 24 insertions(+)
     create mode 100644 readme.md

######Commit new Changes To But...
This time we are going to create new feature branch using git flow commands.
>  notice that Feature branches will take the feature branch name and use that as the pre-release tag.

    λ git flow feature start docs/init
These are the results from executing this command:

    λ git flow feature start docs/init
    Switched to a new branch 'feature/docs/init'
    
    Summary of actions:
    - A new branch 'feature/docs/init' was created, based on 'develop'
    - You are now on branch 'feature/docs/init'
    
    Now, start committing on your feature. When done, use:
    
     git flow feature finish docs/init
    

