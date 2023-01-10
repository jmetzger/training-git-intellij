# 3-Schritte zum Löschen Pull-Request integration 

```
git checkout master 
git pull --rebase origin master 

# Davor: Online branch (neuer feature-branch löschen) 
# Löscht Schattenbranch 
git fetch --prune 

# Und lokaler branch löschen 
git branch -d feature/mein-feature-branch 

```
