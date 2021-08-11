# jupyterlab-git-demo
This is simple demo repository for getting familiar and testing the [jupyterlab-git extension](https://github.com/jupyterlab/jupyterlab-git/tree/jlab-2). 

## Used versions

- jupyterlab:  2.3.1
- git:         2.25.0

## Collaborating on Notebooks
A simple example workflow: 

- create a new (or use existing) branch (e.g. `dev`) to propose changes to a notebook 
- commit, push and start a pull-request in GitHub (to merge in the `main` branch)
- others can pull and inspect the changes in their notebooks
- if o.k. merge the pull-request into the main
- if there are merge conflicts (e.g. changed cell id's) and we know that we want all the changes from `dev` to be incorporated into the `main` do the merge via command line and use the `Xtheirs` merge strategy:

```
git fetch origin
git checkout main
git merge -Xtheirs --no-ff dev
git push
```
