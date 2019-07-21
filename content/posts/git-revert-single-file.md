---
title: "Git revert a single file"
date: 2019-07-21T08:50:14+03:00
tags: ["git", "checkout", "revert file"]
slug: "git-revert-single-file"
description: "Discard uncommitted changes in a single file with the copy in your latest commit."
---
Discard uncommitted changes in a single file with the copy in your latest commit.

```
$ git checkout -- your/filepath
```
<!--more-->
`$ git status` command output has a hint
```
$ git status
On branch master
Your branch is up-to-date with 'origin/master'.
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   your/filepath
 ........
```

 To revert file from particular commit 95919f
```
 $ git checkout 95919f -- your/filepath
```
or one commit before 95919f
```
 $ git checkout 95919f~1 -- your/filepath
```

#### Links
[Git checkout](https://git-scm.com/docs/git-checkout).