## Comandos
Comandos uteis que encontrei, que pode me ajudar na utilização do Git.

### Comandos Autoexplicatorios:

    git --version
    git --help
---
### Comandos com certa necessidade a depender do caso:
    git init - Start a new repository to enable versioning.
    git add - Group related changes together in the staging area, in preparation to "commit" them to history.
    git commit - Save or "commit" the changes in the staging area to the project's history.
        commit message - A short description of the changes to help keep the history organized.
    git status - View the current state of your working directory and staging area.
    git checkout - Change your working directory to a different version from the repository history.
---
### Comandos de visualização de registro
    git log - Display a detailed history of the project.
        git log --oneline - Show one commit per line, but with less detail.
        git log --graph - Show a visual diagram, useful for diverging paths.
    git checkout - Move to a different point in the history (modifies files in your working directory).
---
### Comandos que mostram a diferença entre os estagio de desenvolvimento.

    git diff - Differences between the working directory and the staging area.
    git diff --staged - Differences between staging area and previous commit.
    git diff HEAD~1 - Differences between current commit and previous commit.
---

### Comandos de Branch

    git branch my-new-feature - Start a branch from the current branch.
    git checkout my-new-feature - Change your working directory to a different version from the repository history.
    git merge - Apply the commits from one branch onto another branch. (Default: Fast forward merge)
