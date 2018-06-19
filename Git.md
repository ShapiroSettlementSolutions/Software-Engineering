## Official Hand book
https://guides.github.com/introduction/git-handbook/

           
workspace ------------> index ---------> local repository --------> remote respository
           add                  commit                     push
           commit -a
<-------------------------------------------------------------------------------------
                  pull or rebase
                                                  <-----------------------------------
                                                            fetch
                                                      
                 
           
# Example: Start a new repository and publish it to GitHub

git init [my-repo]    

cd my-repo (change into the `my-repo` directory)

touch README.md       (create the first file in the project)

git add README.md (add it to index)

git commit -m "add README to initial commit"

git push --set-upstream origin master



# Example: Contribute to an existing repository

git clone https://github.com/me/repo.git

cd repo

git branch my-branch

git checkout my-branch

git add file1.md file2.md


git commit -m "my snapshot"

git push --set-upstream origin my-branch


# Example: Remove files\folders

git rm --cached file1.txt

git commit -m "remove file1.txt"

git push origin master  
