# newtemplate
new website designs, templates explored and hammered out here

## Testing themes

[Knight](Knight/)

[Onepage](OnePage/)

## Initation log
* Nikhil: Sharing as this might be useful for folks like me using the command line way of syncing with github for the first time.
* Had the folder locally and had initiated the repo online
* Followed instructions here: <https://help.github.com/articles/adding-an-existing-project-to-github-using-the-command-line/>
* Local folder, opened terminal there and ran these commands
```
$ git init
$ git add .
$ git commit -m "First commit"
$ git remote add origin https://github.com/datameet-pune/newtemplate.git
$ git remote -v
```
* Then, got an error when I went to push whatever I had here up to github, because over there it had already been initialized with a readme file. So I had to pull that commit up there, down to my local folder first: (got this info from <https://stackoverflow.com/a/10510482> )

```
$ git pull --rebase https://github.com/datameet-pune/newtemplate.git master
From https://github.com/datameet-pune/newtemplate
 * branch            master     -> FETCH_HEAD
First, rewinding head to replay your work on top of it...
Applying: First commit

```

* Now we're in sync. Redid commit commands. Skipped the setting up of remote repo as that's already been done. And now I "pushed" it.

```
$ git add .
$ git commit -m "First commit"
On branch master
nothing to commit, working directory clean

$ git push origin master
Username for 'https://github.com': answerquest
Password for 'https://answerquest@github.com': 
Counting objects: 169, done.
Delta compression using up to 2 threads.
Compressing objects: 100% (167/167), done.
Writing objects: 100% (169/169), 16.12 MiB | 53.00 KiB/s, done.
Total 169 (delta 18), reused 0 (delta 0)
remote: Resolving deltas: 100% (18/18), done.
To https://github.com/datameet-pune/newtemplate.git
   815f710..9bee84a  master -> master
```

* And now when I see the repo <https://github.com/datameet-pune/newtemplate> : It's all there :)

#### Clarifications on local-to-remote syncing
* There's no need for your local folder to be named the same as your github repo.

#### Subsequent changes, commits to push up to github
```
$ git add .
$ git commit -m "explanation"
$ git push origin master
```

#### If repo has been changed online, and you want your local folder to sync with it
```
$ git pull origin master
```
