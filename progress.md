## Day 1 — 

**Topic:** Git & GitHub — Branching, Merging, Conflict Resolution & `.gitignore`

**What I Did:**

* Watched Kunal Kushwaha’s **Complete Git and GitHub Tutorial** from the DevOps Bootcamp.
* Practiced the complete local Git workflow using `git init`, `git add`, `git commit`, `git status`, and `git log`.
* Created and switched between branches using `git branch`, `git checkout`, and `git switch`.
* Created a test branch, made changes, and merged it back into `main`.
* Intentionally created a **merge conflict** by modifying the same line differently on two branches.
* Resolved the conflict manually by editing the conflict markers and choosing the correct final content.
* Practiced remote GitHub operations: `git remote`, `git push`, `git pull`, and `git clone`.
* Created a `.gitignore` file and verified that Git correctly ignored files matching the specified patterns.

**Commands & Concepts Learned:**

* `git checkout -b <branch>` / `git switch -c <branch>` — creates a new branch and switches to it.
* `git merge <branch>` — merges the specified branch into the current branch.
* `<<<<<<<`, `=======`, `>>>>>>>` — conflict markers added by Git when conflicting changes are detected.
* **Conflict resolution:** Manually edit the conflicting section, remove the markers, run `git add`, and then commit the resolved changes.
* `git log --oneline` — displays a compact view of the commit history.
* `.gitignore` patterns such as `*.log` and `__pycache__/` — prevent matching untracked files from being added to Git. They do **not** remove files that are already being tracked.

**Stuck On / Key Learning:**

* Initially, I wasn't fully clear about why `git add` is required again after resolving a merge conflict.
* Now I understand that `git add` tells Git that the conflict has been manually resolved and stages the resolved version so the merge can be completed with a commit.
