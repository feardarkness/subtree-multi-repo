# Git Subtree

## Getting started

- Add the remote (replace remote-name-here with the name of the remote and place the correct repository)
```
$ git remote add -f remote-name-here git@github.com:feardarkness/child2-multi-repo.git
```

- Add the remote repositories (name from the previous step) to a folder in the current repository. E.g.: Adding the previous repository to the *.repos/events* folder in the *main* branch.
```
$ git subtree add --prefix .repos/events remote-name-here main --squash
```

## Update subtree


```
# Updating the subtree from the *main* branch
$ git fetch remote-name-here main

# pull from the remote (*main* branch)
$ git subtree pull --prefix .repos/events remote-name-here main --squash
```


