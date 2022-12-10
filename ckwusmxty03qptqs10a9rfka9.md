# How to Contribute to an Open Source?

## Are you a beginner to Open Source?

Doesn’t have an idea for the buzz words PR, issue, commit, push, pull if so check this blog and learn how to contribute to an open-source.



## What is an Open Source?

An Open source is a platform where many people from all over the world work on a project. When a project is open-source, anybody is free to use, study, change, and distribute your project for any purpose. E.g. Linux is an Open-source.



## Why Open Source?

Contributing to open source can be an awarding way to learn, teach, and build experience in any domain. https://ranawattech.hashnode.dev/how-to-contribute-to-an-open-source

## Why do people contribute to an Open Source project?


- 
Brush up on existing skills


- 
Get to work on real-world projects


- 
Meet various people and collaborate



## How to publish an issue?

![Annotation 2021-12-06 203640.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1638803324658/WGX0Mr_fQ.png)


By clicking the issue you will be navigated to the page where you can see a button called new issue


![Annotation 2021-12-06 204527.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1638803744044/wjgB_bWHz.png)




Click the New issue you will be navigated to a comment box at that box, comment what you like to change in the repository, and submit the issue, once they accept the issue given by you they will assign you to contribute to the project.



![Annotation 2021-12-06 204937.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1638803996653/SbHx59Ksp.png)



## Contribution:

Now after they assign, you can start contributing check the following workflow to complete your first contribution. 👇🏻


### Step 1: Haven’t you installed Git? 

 Install now.


### Step2: Fork this repository

It is done by clicking on the fork button on the top right of the page. This will create a new copy of this repository in your account.


![Annotation 2021-12-06 235755.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1638815360879/8ykyf0OCl.png)


### Step3: Clone repository

You can clone the repository by clicking the drop-down button and copying the URL


![Annotation 2021-12-06 233515.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1638813998664/QsCtkiXzP.png)

```
git clone "copied URL"

```
For e.g.

```
git clone "https://github.com/RanawatTech/Android_Frontend_Java.git"

```
Here, Android_Frontend_Java is the name of the original repository now it is locally cloned to your device.

```
cd Android_Frontend_Java

```

The Android_Frontend_Java is your folder name. Now create a branch using the git checkout command:

```
git checkout -b add "branch name"

```

E.g.

```
git checkout -b new_branch

```

Here the new branch is the name of the branch you can give any name it is up to you.


### Step 4: Commit


Now, you can make necessary changes, e.g. You can create a folder called Blog/README.md and insert some text, code and save the file, Now move back to the terminal and give the command

```
git status

```

Now, it lists out the changes you have made.

```
git add 

```

This command helps to add all the changes you have made

```
git commit -m "first commit"

```

This command helps you to commit all the changes you have made to the file, It is not necessary you should name it as the first commit you can also name it as


```
git commit -m "new_branch - readme"

```

The new branch represents your branch name and the readme is the name of your file.


### Step 5: Push Changes

Until now the changes have not been added to the GitHub repository,


```
git push -u origin <add-your-branch-name>

```

E.g.

```
git push -u origin new_branch

```

### Step 6: Submit your changes for review

This is the step where you inform the owner of the repo to accept the changes, which is called PR - Pull request, After pushing the changes move to your cloned repo and refresh the page

//img

Click the compare and pull request and you'll be moving to the comment section

//img

Now comment on your changes e.g. I had fixed the readme file and clicked the create a pull request. Soon when the owner merges all your changes into the master or main branch of the project. You will get a notification email once the changes have been merged.

Bravo! You completed the standard workflow issue ->fork -> clone -> edit -> pull request, Now you can start contributing to open-source projects.











