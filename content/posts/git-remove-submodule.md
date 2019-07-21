---
title: "Git remove submodule"
date: 2019-07-21T18:07:39+03:00
tags: ["git", "remove submodule", "gist"]
---

{{< gist myusuf3 7f645819ded92bda6677 >}}
<!--more-->
Another suggested way that I didn't try.
```
git submodule deinit <path_to_submodule>
git rm <path_to_submodule>
git commit-m "Removed submodule "
rm -rf .git/modules/<path_to_submodule>
```

#### Links
[git-submodule docs](https://git-scm.com/docs/git-submodule) and
[https://gist.github.com/myusuf3/7f645819ded92bda6677](https://gist.github.com/myusuf3/7f645819ded92bda6677)

