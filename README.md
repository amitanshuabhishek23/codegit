**git config --global user.name "Amitanshu"** // Use configure the name globally

$$
git config --global user.email "amitanshu.abhishek@gmail.com" // Use to configure email
$$ 

###### git config --global core.editor "code --wait" // Use to open code editor if there is any issue with the code 

https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line // If code is not set in your zsh profile 

```python
cat << EOF >> ~/.zprofile
# Add Visual Studio Code (code)
export PATH="\$PATH:/Applications/Visual Studio Code 3.app/Contents/Resources/app/bin"
EOF
```


git config --global coe.autocrfl "input" // To configure the line ending that can sync between Windows and Mac OS

git config --global -e   // Edit the global config 


Git Statges : 

U -- untracked 
A - Added or staged 
C - Committed 

git log --oneline -- To check all the checkpoints -- all the commits.  -- Saved points 


git reset --hard HEAD~1 -- To go back to the previous commit

git status -s -- To check on status || To check the status of the added file or committed file 

git log -- to get all the commit.  

**Branching** 

```
amitanshu@Amitanshus-MacBook-Pro Code Git % git status -s    
amitanshu@Amitanshus-MacBook-Pro Code Git % git branch feature/navbar
amitanshu@Amitanshus-MacBook-Pro Code Git % git branch
  feature/navbar
* main
amitanshu@Amitanshus-MacBook-Pro Code Git % git switch feature/navbar 
Switched to branch 'feature/navbar'
amitanshu@Amitanshus-MacBook-Pro Code Git % git branch
* feature/navbar
  main
amitanshu@Amitanshus-MacBook-Pro Code Git % git switch main            
Switched to branch 'main'
amitanshu@Amitanshus-MacBook-Pro Code Git % git switch feature/navbar 

amitanshu@Amitanshus-MacBook-Pro Code Git % git switch feature/navbar 
Switched to branch 'feature/navbar'
amitanshu@Amitanshus-MacBook-Pro Code Git % git switch main           
Switched to branch 'main'
amitanshu@Amitanshus-MacBook-Pro Code Git % git merge feature/navbar  


Three Way Merge 
Fast Forward Branch 

```


```
amitanshu@Amitanshus-MacBook-Pro Ritesh % git clone https://github.com/amitanshuabhishek23/codegit.git
Cloning into 'codegit'...
remote: Enumerating objects: 11, done.
remote: Counting objects: 100% (11/11), done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 11 (delta 0), reused 11 (delta 0), pack-reused 0
Receiving objects: 100% (11/11), done.
amitanshu@Amitanshus-MacBook-Pro Ritesh % git codegit 
git: 'codegit' is not a git command. See 'git --help'.
amitanshu@Amitanshus-MacBook-Pro Ritesh % cd codegit 
amitanshu@Amitanshus-MacBook-Pro codegit % ls
README.md       index.html      script.js       style.css
amitanshu@Amitanshus-MacBook-Pro codegit % git switch -C feature/mar          
Switched to a new branch 'feature/mar'
amitanshu@Amitanshus-MacBook-Pro codegit % git add .
amitanshu@Amitanshus-MacBook-Pro codegit % git commit -m "Adding H1"
[feature/mar 46c6d96] Adding H1
 1 file changed, 1 insertion(+)
amitanshu@Amitanshus-MacBook-Pro codegit % git push -u orgin feature/mar
fatal: 'orgin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
amitanshu@Amitanshus-MacBook-Pro codegit % git push -u origin feature/mar
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 321 bytes | 321.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'feature/mar' on GitHub by visiting:
remote:      https://github.com/amitanshuabhishek23/codegit/pull/new/feature/mar
remote: 
To https://github.com/amitanshuabhishek23/codegit.git
 * [new branch]      feature/mar -> feature/mar
branch 'feature/mar' set up to track 'origin/feature/mar'.
amitanshu@Amitanshus-MacBook-Pro codegit % 

````