## Work Flow For Individual's Projects

**You think you are ready to create a coding project and you want to keep track of the work you have made. Here is a simple work flow for a beginner.**

### Setting up Github Repository

1. Assume you already have a Github account, you can create a new repository by clicking this plus button.

   ![AddRepo](/Img/create-repo1.png)

2. After you create the repo, lets get started with connecting your local project with the Github repo.

   - To do this, first you need to create a project folder on your local machine.
   - Scroll down then you will see the following:

     ![ConnctRepo](/Img/connect-repo.png)

   - We will be using the first one. When you opened your VSCode, redirect your terminal to your project's root directory, copy and paste the whole command into it. Remember the path for `git remote add origin` will be different on yours.

   - After that is done, you can refresh your Github page, and you should see a README.md file with first commit message next to it.

### Start Coding

**YAY! you have connect your project to the Github repo, we can now start our work flow.**

If you have not read about the [Basic Git Command](./GitCommand.md) page, you can check to see what each commands do as you follow these steps.

<hr>

First of all, `main` branch is the branch you want to keep the most up-to-date working code as you work on the project. That being said, you do not want to break the project when you push something that doesn't work on `main`. Therefore, here comes the importance of utilize `branches` for new functionality you are working on. To do that, you can create a new branch from main by doing:

```
git checkout -b your-branch-name
```

What this does is that it will not only build a new branch from main, but will also redirect you into this newly created branch.

Once you finished your code in this branch and by finish, it does not break your program. You can now do git commands such as (`add`, `commit`, and `push`).

![DemoPush](/Img/demo-push.png)

You might have noticed a command appeared as you tried to push like this:

```
git push --set-upstream origin working-code-branch
```

This error is to warn you that you do not have this branch in your repository. To fix this error is simply run the command in your terminal.

After you run the command, the branch should appear in your repository like this:

![PushedBranch](/Img/pushed-branch.png)

Now back in your VSCode, you can change to your main branch by doing:

```
git checkout main
```

and merge your branch into main

```
git merge working-code-branch
git push
```

You will need to `push` again after you merged your branch into main because when you merged, it only merged on your local machine.

Finally, you should see the most up-to-date code on your main branch in Github!

![MergeSuccess](/Img/merged-success.png)

<hr>
Continue Reading:

[[Basic Git Commands](./GitCommand.md)]
[[Team Work Flow](./TeamWorkFlow.md)]

[back to main page](../README.md)
