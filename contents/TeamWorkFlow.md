## Basic Work Flow While Working In A Team

**You think you are ready to create a team project with other people after you have read the flow for individual work, but you are not sure how you can work on the code together and not having code conflicts with your teammates. This tutorial is for you to get started on team work flow.**

### Github Setup For Collaboration

If you have not created a repo, please read [Setting up Github Repository](./AloneWorkFlow.md) here before you continue.

1. Assumed you are the owner of the repository. You can go to `setting` in your repository:

   ![Setting](/Img/setting-button.png)

2. And click on `collaborator`. You will be prompt to sign in again. After that, you will see this page:

   ![collaborator](/Img/collaborator.png)

You can now add teammates to this project in `Manage access`.

### Get Team Members On The Same Page Before Coding

After you or your teammates have been granted access to the repository. Here are the steps you or your team can follow to get the project onto your local machine.

1. Go to the `main` branch in Github and find this https link under green `Code` button.

   ![clone](/Img/clone-repo.png)

2. If you are not the repository creator, you will need to copy and paste the link with this command and run:

   ```
   git clone replace-the-link-here
   ```

3. Now you should have the project in your local machine and ready to follow the work flow as you work on the project.

### Work Flow

The following work flow is for developers who already have knowledge of work flow individually [here](./AloneWorkFlow.md) and a continue flow built based on it.

In the most up to date branch (main):

1. create a new branch:
   ```
   git checkout -b <branch-name>
   ```

## From here on is when you think your code is ready for a merge

2. start coding, before you proceed to push your code, To check if you accidentally modify other files
   ```
   git status
   ```
3. To double check which branch you are on (**make sure it's not main branch**):
   ```
   git branch
   ```
4. to add the new change that you want to commit:

   ```
   #for all change made
   git add .
   git add -A
   ```

   or

   ```
   #for a file
   git add <filename>
   ```

5. to commit changes (add description on the changes)<br/>
   you can do this as many time as you want before step 6

   ```
   git commit -m "<your description on the change>"
   ```

6. Make sure you are NOT in the main branch before you push your code
7. when you are ready to request a PR, push your code to the remote repo:

   ```
   git push
   ```

   it will then give you a command line that looks like

   ```
   git push --set-upstream origin <your branch name>
   ```

   you can just copy and paste and run that command

8. go to the github repo
9. click create pull request top of the repo
10. assign the reviewer to anyone working on the code
11. assignee as yourself, then create the pull request, click
    [here]("https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request") for additional PR info.

## Additional git note:

### To modify current branch name

```
git branch -m <new branch name>
```

### To delete a branch:

(You will have to be outside of that branch)

local:

```
git branch -d
```

remote:

```
git push --delete origin <branch name on remote>
```

### Switch between branches

```
git checkout <branch name>
```

<hr>
Continue Reading:

[[Basic Git Commands](./contents/GitCommand.md)]
[[Alone Work Flow](./contents/AloneWorkFlow.md)]

[back to main page](../README.md)
