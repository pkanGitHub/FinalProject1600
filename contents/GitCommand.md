## Different Git commands or VSCode Interface You Want To Know Before Starting

**In this section of the tutorial, you will learn about the most basic git commands you want to get familiar with before you start to work on a project with Github.**

### Using Commands

<hr>

```
git add .
```

Move changes from local directory to staging area.
The (`.`) in this scenerio mean you want to include all the changes you made and when you commit, the message will applies to all the files.

```
git add <your file name>
```

OR you can specify which file(s) you want to add, in this case, you can add different messages to different files.

<hr>
 
```
git commit -m "<your message goes here>"
```
Make a note/message to what you have done in this/these files you added

<hr>

Push the changes to remote repository

```
git push
```

<hr>

Switch to different branches

```
git checkout <branch-name>
```

OR if you want to build a branch, you can add a `-b` flag before branch name.

<hr>

To pull the most up-to-date code from Github to local machine.

```
git pull origin main
```

Often time, you can simply do `git pull` if you are already on the main branch on your local machine.

<hr>

```
git branch
```

This command is to look for branches names. This is default to show all the branches you have created in your computer. Most often it is use to see which branch you are currently in.

### Using VSCode Interface

1. **To add changes for staging:**

   Click on the `source control` icon. It will display a list of changes you have made in your project. You can add all or just single file.
   Once you click on the `+` button, it will add the change for staging.

   ![SourceControl](/Img/git-add.png)
   ![AddChanges](/Img/git-add2.png)

2. **Commit changes:**

   Here is where you type in your messages for the change you are planning to add to remote repository.

   ![CommitChanges](/Img/git-commit.png)

3. **Push changes:**

   To push changes, go to the `...` on the top right corner and find `Push` option. Once you click on it, the file that you added to `staged changes` will be saved onto your repository in Github.

   ![Push](/Img/git-push.png)

4. **Voila ~**

   ![github](/Img/github-page.png)

### Continue Reading:

[[Alone Work Flow](./contents/AloneWorkFlow.md)]
[[Team Work Flow](./contents/TeamWorkFlow.md)]

[back to main page](../README.md)
