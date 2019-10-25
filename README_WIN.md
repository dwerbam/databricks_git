# INSTALLATION OF dbgit ON WINDOWS

## pre-requisites
1. install miniconda
1. install git
- make sure git is configured:
> git config --global user.email "you@example.com"

> git config --global user.name "Your Name"

## installation steps
1. enable "bash" in the path, add "C:\Program Files\Git\bin" to the Windows path Env System Variables
1. activate the python environment, start anaconda prompt from windows>start
1. install and configure databricks-cli:
> pip install databricks-cli

> databricks configure --token

- in conda activated environment run: 
```
bash
```

```
mkdir "$HOME/bin"
curl "https://raw.githubusercontent.com/dwerbam/databricks_git/master/databricks_git" > "$HOME/bin/dbgit"
```

(at this point you have dbgit installed and running.. just run 'dbgit' to test it)

## How to use it:
```
mkdir ~/localdev
cd ~/localdev
dbgit init "/DEV"
dbgit pull
```
