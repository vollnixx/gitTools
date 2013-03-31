# checkGitDirs
* checkGitDirs is a simple bash script which checks the local git repositories for uncomitted files
* ignore function for git repositories which should not be listed

To run the script you must have installed **git** and **locate**.
If the script is not executable type into your shell:

    chmod u+x checkGitDirs
    
If newer repositories are not listed you should first refresh your file database with the following:

    sudo updatedb
    
Then you can just execute the script with:

    ./checkGitDirs

By default the directories */usr/local* and */var/www* are ignored, if you have directories in there which you want to be checked remove/change the entries from line 8 of the script:
    
    IGNORE="/usr/local|/var/www";
