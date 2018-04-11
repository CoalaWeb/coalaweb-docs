**Note:** This tutorial has been written for **Ubuntu** but with some slightly changes it should be applicable to other operating systems.

## Prerequisites
 - Operating System: Ubuntu (Debian)
 - GIT client installed

## Overview

Sometimes you have already done an initial commit and pushed it before you decided to add something to a gitignore file. In those cases eventhough you have it listed in your gitignore file it will appear in the GitHub project. To keep the file in your local resposiory but remove it from GitHub you can follow these steps.

## Steps

### Project location
Change location to the project directory you wish to make changes to (monitored by GIT)

    cd ~/projects/example-project
  
### Remove Directory  
In this example I added the PHPStorm **idea** directory to the projects **.gitignore** file but it had already been uploaded during the initial commit so to remove it try this:

    git rm -r --cached .idea/
    
The command above will delete the directory content recursively (everything inside, even sub-directories).
 
### Remove Individual files

Single file can be removed like this

    git rm --cached file_1

Multiple files at the same time

    git rm --cached file_1 file_2 file_3 

### Commit changes
Next commit the changes

    git commit -m "Removed folder from repository"

### Push changes
Lastly push the changes entering your github password when prompted.

    git push

## All done
Now over on GitHub if you refresh the page the directory should no longer exist in your project.