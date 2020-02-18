# Git common commands cheat sheet

## CLone

#### Clone a remote repository in local folder
```bash
> git clone {RepositoryLink, ex: https://xxx.git}
```

## Branch

#### Display local branches
```bash
> git branch
```

#### Display all remotes branches information
```bash
> git fetch -a
```

#### Display all remote & local branches
```bash
> git branch -a
```

#### Refresh all local branches information when there are modifications on remote server side, ex: deletion of some branches
```bash
> git remote update origin --prune
```

#### Switch to another branch in local folder
```bash
> git switch {BranchName}
```

## Pull 



## Push

#### Push local commit to remote origin
```bash
> git push
```

## Tag

#### Create a tag from current branch
```bash
> git tag {TagName}
```

#### Push local tags to remote origin 
```bash
> git push origin --tags
```

