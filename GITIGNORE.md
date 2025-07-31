# How To Clean Already tracked files?
If target files e.g. `.DS_Store` or `.sh` were already committed before adding them to .gitignore, Git will keep tracking them until you untrack them.

To stop tracking them:
```bash
# Remove .DS_Store and .sh files from Git index (but keep locally)
git rm --cached **/.DS_Store
git rm --cached **/*.sh

# Then commit
git commit -m "Remove ignored files from tracking"
```
