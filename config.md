# git config

## How to delete an entry from config 

```
# Important: Find exact level, where it was added --global, --system, --local 
# test before
# should contain this entry 
git config --global --list 

git config --unset --global alias.log
```

## Die verschiedenen Ebenen 

```
# user global gesetzt
git config --global user.name "Jochen Blaumann Metzger"
#nur im Repo gesetzt
git config user.name "J. Blaumann"
# Zeig mal was auf Systemebene gesetzt ist (oberste Ebene)
git config --list --system
# Zeige mal, was auf User-Ebene gesetzt ist (2. Ebene)
git config --list --global
# Zeig mal was auf Repo-Ebene gesetzt ist 
git config --list --local
#ä Und was ist das ergebnis ? -> per Vererbung, was nimmst du am Ende
git config --list

# Weclhe email wird jetzt im Repo verwendet 
git config user.email
# Welcher Name wird jetzt im Repo verwendet ?
git config user.name
```

