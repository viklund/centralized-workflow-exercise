

# centralized-workflow-exercise

Exercise to practice collaborative centralized workflow. On the way to a pull request
and code review we will meet and discuss a number of typical pitfalls.


## Before we start

1. Participants add their usernames to a shared document.
2. Instructor adds participants as collaborators to this project.


## After participants have been added as collaborators


### 1. Clone this repository

If you have set up ssh keys:
```
$ git clone git@github.com:coderefinery/centralized-workflow-exercise.git
```

If you have not set up ssh keys:
```
$ git clone https://github.com/coderefinery/centralized-workflow-exercise.git
```


### 2. Step into the newly created directory:

```
$ cd centralized-workflow-exercise
```


### 3. Create a file with a unique name, e.g.: `yourusername.txt`

In this file share your favourite cooking recipe or haiku or Git trick or whatever.


### 4. Stage and commit the change

```
$ git add yourusername.txt
$ git commit
```


### 5. Try to push the change to the upstream repository

```
$ git push origin master
```


### 6. **Stop here** and discuss why push for most participants was rejected

It will work only for one participant. Why?


### 7. Pull updates from the upstream repository

```
$ git pull origin master
```


### 8. **Stop here** and discuss why we obtained a merge commit locally

Ideas? What happened under the hood? Discuss `git fetch` as an alternative to `git pull`.
Discuss `git pull --rebase` as an alternative to avoid merge commits.


### 9. Try to push again

It will work for one more person.


### 10. Create a branch `yourname/somefeature` pointing at your commit

```
$ git branch yourname/somefeature
```


### 11. Push your change as a new branch

```
$ git push origin -u yourname/somefeature
```

Can we leave out the `-u`?


### 12. Submit a pull request

Submit a pull request from your branch towards the `master` branch.
Do this through the web interface.


## After the exercise

1. Instructor removes collaborators.
2. Instructor rewinds the repository to the state before the exercise.
