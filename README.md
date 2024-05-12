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
