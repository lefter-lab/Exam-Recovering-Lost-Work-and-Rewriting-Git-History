Since I don't know how you will identify me in SoftUni, because my username there is already taken on GitHub, I will write my SoftUni username here – lefty, my real name (Todor Lefterov), and my email lefter@abv.bg.

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
