# Basic Starting Working with Repositories Guide

### Prerequisites

What things you need to do/have in order to work with git?

```
* Available command line (terminal), bash o zsh for macOS o Linux, MSysGit for windows
* Install git --> https://git-scm.com/book/es/v2/Inicio---Sobre-el-Control-de-Versiones-Instalación-de-Git
* Check `git version` in command line to make sure it's installed
* Create github account --> https://github.com/join
* Generate ssh key - Generar un ssh key ---> https://help.github.com/es/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent o https://git-scm.com/book/es/v2/Git-en-el-Servidor-Generando-tu-clave-pública-SSH
* Connect with github account https://help.github.com/es/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account
```

## Hands on

* Navigate to some directory in the command line and type `git clone git@github.com:jeffveleze/test-repository.git`
* Even if this repo is public reading access, editing is not, so please request access and i will allow to edit it
* Open one of the text files inside of the folder cloned and do some change on it. Save and exit
* In the command line, do `git add .`, then `git commit -m "Any message which indicates the change"`, then `git push origin master`. You can see now your changes being published in the remote repository
* Create a branch doing `git checkout -b "branch-name"`, then repeat the last 2 steps but instead of pushing to master, push to the branch-name
* In order to merge that branch into master you need to go to master doing `git checkout master` and then type `git merge branch-name` 
* To delete you branch locally type `git branch -D branch-name`
* To discard changes without being commited type `git checkout -- .`
* To see current no commited changes you can type `git diff`

## Authors

**Jeff Velez**

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
