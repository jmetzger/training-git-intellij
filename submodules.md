# Submodules best practice 

## Walkthrough 

```
# uses the same branch as main repo 
git submodule add https://github.com/jmetzger/training-git-pycharm

# tracking is done here:
# cat .gitmodules 

```

## clone repo with submodules (done afaik automatically by pycharm) 

```
git clone --recurse-submodules --remote-submodules <repo-url>

```

## Updating commands for updating subfolder 

```
git submodule update --remote 
# use other branch from submodule then master 
git config -f .gitmodules submodule.training-git-pycharm.branch stable
```

## Task: Set submodule to a specific tag 

```
cd submodule_directory
git checkout v1.0
cd ..
git add submodule_directory
git commit -m "moved submodule to v1.0"
git push
```


## Ref.

  * https://git-scm.com/book/de/v2/Git-Tools-Submodule
