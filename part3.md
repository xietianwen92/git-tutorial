    # now suppose Bob also join the development team
    # Bob clone a copy with full history from the remote repository
    # into a new location

    git clone /path/to/remote/myRepo.git BobRepo


    # go to newly cloned repo and check history
    git status
    gitk
    git branch

    # Bob makes changes to wordcount.py
    # On line 76 , change 20 to 30
    # Bob commits the change
    git commit -a -m "increased the number of topcount results"

    # push the change to remote repository
    git push origin master


    # now go back to your first local repository (Alice)
    # you also make a change to wordcount.py:
    # change line 77 to
        print item[0] + ' has appeared ' + str(item[1]) + ' times'

    # commit the change 
    git commit -a -m "reword the program output"

    # push to the repository
    git push origin master

    # You get an error, telling you that there is already a change
    # made on the remote server. pull the update
    git pull origin master

    # Git automatically merge the changes that Bob did to your repository
    # and commit this auto-merge

    # Now push the change to the remote repository
    git push origin master



