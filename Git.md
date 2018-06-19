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
create a new directory, and initialize it with git-specific functions
git init [my-repo]

change into the `my-repo` directory
cd my-repo

create the first file in the project
touch README.md

git isn't aware of the file, stage it
git add README.md (add it to index)

Commit notes
git commit -m "add README to initial commit"

push changes to github
git push --set-upstream origin master



# Example: Contribute to an existing repository
download a repository on GitHub.com to our machine
git clone https://github.com/me/repo.git

change into the `repo` directory
cd repo

create a new branch to store any new changes
git branch my-branch

switch to that branch (line of development)
git checkout my-branch

make changes, for example, edit `file1.md` and `file2.md` using the text editor

stage the changed files
git add file1.md file2.md

take a snapshot of the staging area (anything that's been added) /add notes
git commit -m "my snapshot"

push changes to github
git push --set-upstream origin my-branch


# Example: Remove files\folders
git rm --cached file1.txt
git commit -m "remove file1.txt"
git push origin master  
