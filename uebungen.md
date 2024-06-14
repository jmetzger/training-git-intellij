# Übungen im Training 

```
## Übung 11 

1. Trainer legt Gruppenprojekt an und pushed code
2. Gruppenprojekt clonen 
3. Zugriff über gitlab testen:
https://gitlab.com/training.tn1/bbgruppe1/
4. feature-branch erstellen

feature/jochen1 

5.  eine neue datei anlegen + adden +committen 

6. feature  - branch pushen 

7. merge-request 


--- nacheinander 
8. mergen

--- aufräumen 
9. wechseln in den master 
10. master pull (löscht er den schattenbranch)  
11. feature - branch 


## Übung 10

1. lokal: neuen Branch feature/4840
2. Ändern README.md Zeile 1 + add + commit 
3. Ändern datei2.txt + add + commit 

4. Online in master: neuen ánhänge readme
committen 

5. Online in master: Zeile 1  readme
committen 

6. Änderungen von Online mit pull --rebase abholen 

---

7. dann feature pushen 

8. merge request 

9. Aufräumen 
a. in master wechseln 
b. git pull master
c. feature-branch löschen 




## Übung 9c 

1. feature/4836 pushen 
2. merge requests
3. mergen 

3.5 Anschauen im graphen online 

4. aufräumen 
a. in den master wechseln
b. pull --prune
c. feature löschen 

## Übung 9b

1. lokal: neuen Branch feature/4836 
2. Ändern datei1.txt + add + commit 
3. Ändern datei2.txt + add + commit 

4. Online in master: neuen ánhänge readme
committen 

5. Online in master: neuen ánhänge readme
committen 

6. Änderungen von Online mit pull --rebase abholen 

---

7. dann feature pushen 

8. merge request 

9. Aufräumen 
a. in master wechseln 
b. git pull master
c. feature-branch löschen 


## Übung 9a

1. lokal: neuen Branch feature/4835 
2. Neue datei1.txt + add + commit 
3. neue datei2.txt + add + commit 

4. Online in master: neuen ánhänge readme
committen 

5. Online in master: neuen ánhänge readme
committen 

6. Änderungen von Online mit pull (merge) abholen 

7. dann feature pushen 

8. merge request 

9. Aufräumen 
a. in master wechseln 
b. git pull master
c. feature-branch löschen 


## Übung 8: neues feature mit merge-request (mit Konflikt) 

1. Online in master -> README.md Zeile 1 ändern 
--

2. Lokal: Neuen branchen feature/4832 
3. Ändern Datei README.md Zeile 1 ändern + add + commit 
4. git push -u origin feature/4832 

5. Online: Merge Request  erstellen 

-> Conflict 

5.5. Konflikt lösen 
a. Die Änderung lokal abholen (vom master)
b. Conflict lösen
c. Mergen lokal 
d. noch pushen 


5.6. und mergen 


6. Aufräumen
6.1. master wechseln udn auf 'n Stand bringe 
6.2. pull --prune // schattenbranch löschen (Remote Tracking Branch)
6.3.  lokalen feature-Branch löschen 





## Übung 7: neues feature mit merge-request (ohne Konflikt) 

1. Lokal: Neuen branchen feature/4831 
2. Lokal neue Datei f1.txt erstellen + add + commit 
3. Lokal neue Datei f2.txt erstellen + add + commit 
4. git push -u origin feature/4831 

5. Online: Merge Request  erstellen 
5.5. und mergen 


6. Aufräumen
6.1. master wechseln 
6.2. pull --prune // schattenbranch löschen (Remote Tracking Branch)
6.3.  lokalen feature-Branch löschen 
c. master auf Stand bringe 



## Übung 6:(Online und lokale Änderung) 

1. Online: README ändern -> Zeile 1 
2. Lokal Datei README -> Zeile 1 
+ add + commit
3. Push 
4. Konflikte  lösen
5. Nochmal pushen 


## Übung 5:(Online und lokale Änderung) 

1. Online: README ändern
2. Lokal neue Datei AGENDA.md mit einer Zeile 
+ add + commit
3. Push 




## Übung 4: (Onloneänderung ohne Konflikt) 
    
    1. Online: Ändern der README 
    2. Lokal: Änderung abholen 
    
    



## Übung 3: Übung reset 

1. Auf alten Stand zurück in intellij über log
2. auf kommandozeile gehen und mit reflog letztes commit 
vor reset ausfindig machen
3. git reset --hard <zu-id-aus-2>
4. Überprüfung des Logs in Intellij 


## Übung 2: Konflikt mit mergetool 

1. You are in master-branch
2. Checkout new branch feature/4722
3. Change line1 in README.md
4. git add -A; git commit -am "done"
5. Change to master 
6. Change line1 in README.md

7. git add -A; git commit -am "change line1 in README in master" 

8. git merge feature/4722


## Übung 1: Konflikt 

1. You are in master-branch
2. Checkout new branch feature/4721 
3. Change line1 in README.md
4. git add -A; git commit -am "feature-4721 done"
5. Change to master 
6. Change line1 in README.md


7. git add -A; git commit -am "change line1 in todo.txt in master" 

7.5. Tiefsinnige Betrachtung -> Log 


8. git merge feature/4721

```
