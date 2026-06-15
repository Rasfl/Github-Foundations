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

---
### Comandos de DIFF


| Comando                     | Função                                                                                                              |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| git diff                    | Mostra as alterações no diretório de trabalho que ainda não foram adicionadas ao stage (não foram “git add”).       |
| git diff report.md          | Mostra as alterações não adicionadas ao stage apenas do arquivo report.md.                                          |
| git diff --staged           | Mostra as alterações que já foram adicionadas ao stage (com git add) em comparação com o último commit.             |
| git diff --staged report.md | Mostra as alterações em stage apenas do arquivo report.md, comparando com o último commit.                          |
| git diff 35f4b4d 186398f    | Mostra as diferenças entre dois commits específicos.                                                                |
| git diff HEAD~1 HEAD~2      | Mostra a diferença entre dois commits anteriores ao HEAD (ordem importa: compara o mais recente com o mais antigo). |
---

### Apagando Branchs

| Comandos | Descrição |
| :--- | :---|
|git branch -m feature_dev chatbot | Para alterar o nome de uma branch chamada "feature_dev" para "chatbot"|
| git branch -d chatbot | Serve para apagar a branch "chatbot"|
|git branch -D chatbot| Serve para forçar o apagamento da branch "chatbot"

### Comitando Branch

| Comandos | Descrição |
| :--- | :---|
|git switch main| Mudar para a main|
|git merge ai-assistant| para dar merge da branch ai-assistant para a main (ou para a branch que estiver localizada)|
|git merge ai-assistant main| Para dar merge do ai-assistant para a main|
|||