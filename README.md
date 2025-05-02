# Pull requests and GitHub issues
## PR's (sorry for spelling)
Pull requests (PRs) are like merging to main on Local, but better, since, in a collaborative setting, it allows for code review.
Let's say you made an important change worth being merged into main. You would inevitably push it to the remote development branch, and will see a popup that looks like the following image.
<br>
<img width="600" alt="Screenshot 2024-04-17 at 12 34 05 PM" src="https://github.com/Poleron402/ez_pts_sp24B/assets/89750832/955b1856-f141-4afe-acca-b953e6a1f286">
<br>
This pops up when the branch has something different in it from main. Click the Compare & Pull request button. This will take you to the window where you can describe what changes you made.

<img width="600" alt="Screenshot 2024-04-17 at 12 35 05 PM" src="https://github.com/Poleron402/ez_pts_sp24B/assets/89750832/78434a4e-a392-418a-a8ca-b7d336c3a0fb"><br>
If you have protections set on main branch (ideally), you will not be able to merge on your own - your teammate will have to approve the merge (or, in work setting, a senior developer). Now create the pull request. The following window will pop up. If there are conflicts (which there are none at the moment), they would need to be resolved locally. My usual ritual for resolving is: 
1. On local, `git checkout main`,
2. `git pull origin main` to make sure all is up to date,
3. `git merge feature_branch` into main (we are mimicking what is happening on remote). This will let you know that there are merge conflicts and prompt you to resolve them by picking the version of the files or individual lines of code that is best. Remember, though, to be mindful, as merge conflicts appear when two developers modified the same file with `main` being the recent common ancestor.
4. Then, `git checkout feature_branch` again, since this is the branch we are merging on the remote.
5. `git push origin feature_branch`. Merge conflict message should be gone :)

<br>
<img width="600" alt="Screenshot 2024-04-17 at 12 35 45 PM" src="https://github.com/Poleron402/ez_pts_sp24B/assets/89750832/314c8251-32c3-4030-afbc-dbc9c7c860c2">
<br>
Click merge.
<br>
<img width="600" alt="Screenshot 2024-04-17 at 12 35 56 PM" src="https://github.com/Poleron402/ez_pts_sp24B/assets/89750832/117fa775-26af-4566-832f-b6468731f189">
<br>
And confirm. Now your remote has branches for development, and the main is up to date so your collaborators can pull the most recent changes on their local project.

<hr>
## Issues
Think of issues as of a TODO list but in a GitHub fashion. Issues allow you to pile up your Project TODOs and ideas into one spot.
Let's create one<br>
<img width="700" alt="Screenshot 2024-04-17 at 8 11 43 PM" src="https://github.com/Poleron402/ez_pts_sp24B/assets/89750832/b7b086ea-bbdd-4a9c-b62e-e2de06dc778d"><br>
The next screen will have a big green button that prompts to add a new issue, click it and add an issue.<br>
<img width="800" alt="Screenshot 2024-04-17 at 8 13 37 PM" src="https://github.com/Poleron402/ez_pts_sp24B/assets/89750832/10386b31-346d-4a1f-8424-44bfa72f17be"><br>
Make it descriptive. Now, upon accessing issues tab again, you will see a list of issues that need attention. <br>
<img width="800" alt="Screenshot 2024-04-17 at 8 14 20 PM" src="https://github.com/Poleron402/ez_pts_sp24B/assets/89750832/a597e641-f539-432d-a115-cb7a6492470c"><br>
We can assign that issue to someone to resolve, add flags, or resolve them later.
For example, one issue was to finish this readme, and I'll count it as documentation related. Some other issues could be solving a bug -- for example, imagine you have a null pointer exception occuring somewhere in your program. You can create an issue, tag it as a bug, and assign it to your teammate for resolution. <br>
<img width="800" alt="Screenshot 2024-04-17 at 8 14 25 PM" src=https://github.com/Poleron402/ez_pts_sp24B/assets/89750832/0208d479-3799-43b2-a1f3-a8301bdc2b5e">


<br>
PRs and Issues are great addition to your project as they help with organization and facilitate best practices.
