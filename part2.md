    # create a remote repository (in a different location or on a server)
    mkdir myRepo.git

    # initilze it
    git init --bare

    # copy the address down

    # back in your local directory, add the remote repository
    git remote add origin /path/to/myRepo.git


    # push changes to remote repo
    git push origin master

    # push the other branch
    git push origin release

    # check git status or gitk
    git status







