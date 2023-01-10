# Pushen und Pullen 

## Neuen Branch pushen 

```
git push -u origin neuer-branch 
```

## Unseren lokalen master auf dem Stand mit online master halten

```
git pull --rebase origin master 
```

## Wir arbeiten an einem branch und wollen diesen täglich mit dem master aktualiseren

```
# Initial beim ersten mal damit arbeiten 
git checkout master 
git checkout -b feature/neuer-branch

# danach täglich im feature/neuer-branch 
git pull --rebase origin master
```
