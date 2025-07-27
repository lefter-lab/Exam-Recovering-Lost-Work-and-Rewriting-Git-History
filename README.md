Since I don't know how you will identify me in SoftUni, because my username there is already taken on GitHub, I will write my SoftUni username here – lefty, my real name (Todor Lefterov), and my email lefter@abv.bg.

this is  git reflog history

fed8146 (HEAD -> development, origin/development) HEAD@{0}: commit: first commit
a19af3b (recovered) HEAD@{1}: reset: moving to recovered
f7142f6 (old-version) HEAD@{2}: checkout: moving from recovered to development
a19af3b (recovered) HEAD@{3}: rebase (finish): returning to refs/heads/recovered
a19af3b (recovered) HEAD@{4}: rebase (pick): Day 5: Friday
4e19882 HEAD@{5}: rebase (reword): Workday 4: Implemented new feature
3fe1acb HEAD@{6}: rebase: fast-forward
f7142f6 (old-version) HEAD@{7}: rebase (start): checkout old-version
ec9c8fd HEAD@{8}: checkout: moving from development to recovered
f7142f6 (old-version) HEAD@{9}: reset: moving to old-version
ec9c8fd HEAD@{10}: checkout: moving from old-version to development
f7142f6 (old-version) HEAD@{11}: checkout: moving from development to old-version
ec9c8fd HEAD@{12}: commit: Day 5: Friday
3fe1acb HEAD@{13}: commit: Day 4: Thursday
f7142f6 (old-version) HEAD@{14}: commit: Day 3: Wednesday
38d7145 HEAD@{15}: commit: Day 2: Tuesday
66adc8b HEAD@{16}: commit (initial): Day 1: Monday


# Exam-Recovering-Lost-Work-and-Rewriting-Git-History


## ✅ Objectives

- Recover lost commits using `git reflog`
- Clean up commit history using `git rebase -i`
- Safely force-push changes without disrupting teammates

---

## 🔧 Steps Performed

1. Initialized Git repository and created a `development` branch
2. Simulated a week of work with 5 commits (`Day 1: Monday` to `Day 5: Friday`)
3. Simulated a bad `git push --force` with an outdated state
4. Used `git reflog` to recover missing commits
5. Rebased the recovered commits to clean up history
6. Replaced `development` with the cleaned-up history
7. Pushed changes safely using `git push --force-with-lease`

---

## 📂 Branches

- `development` – main working branch used during the task
- `recovered` – temporary branch used to recover lost commits

---

## 💡 Notes

- `git reflog` is extremely powerful for recovering lost work
- `git rebase -i` is useful for rewriting and simplifying commit history
- Always prefer `--force-with-lease` over `--force` when pushing

---

## ✅ Result

All lost commits were restored, history was cleaned, and the final state was safely pushed.
