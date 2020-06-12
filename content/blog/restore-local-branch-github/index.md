---
title: How to restore local  branch in GitHub?
date: "2020-06-12"
description: "you ended fucking up the re-base so badly that you deleted the repository and cloned a new one 😂"
---

To find out the **`sha`** of the latest commit, run the command :
```bash
$ git reflog
```
<br>

It will provide all the **`HEADs`** of all branches. After this, simply run the command given below to recreate a branch using **`sha`** :

```bash
$ git branch branchName <sha>
```
<br>

**Voila ! This is how you can restore local branches in GitHub 💡**

## WORST CASE :

In my case, I re-installed the OS which resulted in deleting all the local branches of my repository. Even **`git reflog`** was not able to save me this time 😓. I lost **`sha`** of all the commits and all the local branches of my repository. So, after brainstorming, I landed up with the solution described below :

```bash
$ git checkout master
# Switched to branch 'master'

$ git fetch --all
# updates local copies of remote branches

$ git branch -a
# List all your branches

$ git checkout branch-name
# Switched to branch 'branch-name'

$ git log
# View the commit history
```
<br>

**Note :** This solution is also useful if you are cloning the repository on new/other laptop or you ended fucking up the re-base so badly that you deleted the repository and cloned a new one 😂 , which might result in deleting all the local branches of your repository and <i>**worst case**</i>, you even lost **`sha`** of the commits 🤷🏻‍♀️

Happy Git ! ❤️