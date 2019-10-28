# Basic Commands      

Use `Cmder` for windows click [here to download full with git](https://cmder.net)  :-)

- Create new file with the extension -
	```sh
    touch filename.extension
    ```

- Create new folder in current location
	```sh 
    mkdir foldername 
    ```

- `ls` will list out folder & files names of current folder
    ```sh
    ls
    ```

- To remove file from current folder
    ```sh
    rm filename.extension 
    ```
	
- To remove folder from current directory
	 ```sh
    rmdir  foldername 
    ```

# Git



***Initialization***
- Following will initialize an empty git that make `.git ` hidden folder in   current folder
	```sh
        # git init  
    ```
![Git-Stages](https://github.com/yashgandhi2020/gitcheatsheet/blob/master/gitst.png)

***Staging Area***
- Once you modified code then you can add file to `Staging Area`
- Following will show which files are in `Staging Area` with blue color
	```sh
        # git status 
    ```
    - if there is red color then that red color file's are not added in `Staging Area`
    - when you commite something git will commit files from staging area so you have to add files into `Staging Area`
- Following will add file into `Staging Area` 
	 ```sh
        # git add filename.extention 
    ```
- Following will add all file in `Staging Area` 
	
	```sh
        # git add .  
    ```
	- Dot will add `ALL` files to `Staging Area`

# Commit 
	
- Commit is important stag, In that you will commit sll changes and save a check point on it
- here is cmd to commit changes
	```sh
        # git commit -m "Message" 
    ```
	- -m denote Message 

- Following will show all commites, commit number and commit Message that you have done.
	```sh
        # git log 
    ```
- Following will show all commit with commit short number and Message in Oneline

	```sh
        # git log --oneline 
    ```

# undoing: { 1. checkout commit   2. revert commit  3. reset commit }

- Following will give you Commit number
    ```sh
    # git log --oneline
    ```

- Following will give you that time of code and you can compare that code with current code that's why git called as `Version Control`!
	
    ```sh
        # git checkout commitnumber 
    ```
- To come back to latest code 

	```sh
        # git checkout master 
    ```

- it will undo that commit and all changes if you add h3 tag in that commit        it will remove it 
	```sh
        # git revert commit_number 
    ```
- Following will remove all commit till `commit_number` but code remain as it is, there is no change in code 

	```sh
        # git reset commit_number 
    ```
- To remove all code and commit's till `commit_number` here is cmd

	```sh
        # git reset commitnumber --hard 
    ```

# Branches
	
- Till now we were working on master branch, now we will make branches ✌
- What is `Branch` :  Making copy of master branch code { Latest Code } is called branching, So you can play with it without affecting master branch code. 
- To make a branch
    ```sh
        # git branch branchname 
    ```
    - But remember working branch does not change, you are on master barnch
 
- Following will show all branch's with there name 
    
    ```sh
        #git branch -a 
    ```
    - There should be `star` ( * ) before one branch that means you are on that branch 
	
- Following will change branch 

	```sh
        #git checkout branchname 
    ```
- If you want to delete branch then here is cmd but remember you should go to Master branch first

	```sh
        # git branch -D branchname 
    ```
- If you want to create branch and directly want to enter in it without checout
	
	```sh
        #git checkout -b branchname 
    ```
	- -b means new branch

# Mergeing
- If branch code is efficient than master branch code then you can merge it  

	```sh
        # git merge branchname 
    ```
	- it will merge branchname with Master branch but be sure you are on master branch
# GITHUB        

- First create `empty repository` and copy `HTTPS` link

- push to `Github`

- Following will add your project to github.

	```sh
        # git push -u ssh_link/origin branch_name 
    ```
- Following will add name to HTTPS link as origin ( you can give name          whatevs you want )
	
	```sh
        # git remote add origin HTTPSlink 
    ```
	- then push project as
        ```sh
        # git push origin master
        ```

- Follwoing will show which link have name as origin

	```sh
        # git remote -v 
    ```
	
# clone project
	
- TO add project in current folder.
	
    ```sh
        # git clone link 
    ```
	- when you clone the project then remember it auto save link name as       `origin` 

- Following will push code to github

	```sh
        # git push -u origin branch_name 
    ```

# Pull

- Following will fetch all code from github and add it  into branch_name 
	
    ```sh
        # git pull origin/link branchname 
    ```
- Following will push code to master branch code and if your code is efficient than master branch code then you can merge it with master branch code 
			
	```sh
        # git push origin/link branchname 
    ```

# Contribute:

- first fork the request it will copy code to your github account 
- then change the code by pulling in to your machine 
- then push the code
- then click on new pull request 
- and cofirm it!!!

***Happy Coding*** 😉
