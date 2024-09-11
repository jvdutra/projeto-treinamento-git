## GIT FLOW

Git flow é uma ferramenta que facilita os comandos de criação e manipulação de branches, encurtando os comandos.

## comandos iniciais
### FEATURE

    git flow feature start (nomebranch)

cria uma nova branch baseada na **DEVELOP**

automaticamente a nomeia como **feature**/nomebranch

faz o checkout para nomebranch

    git flow feature finish (nomebranch)

faz merge da **feature**/nomebranch na **DEVELOP**

deleta a **feature**/nomebranch

muda para a develop

    git flow feature publish (nomebranch)

publica branch feature no repositorio remoto

### RELEASE

    git flow release start (nomebranch)

cria uma nova branch baseada na **DEVELOP**

automaticamente a nomeia como **release**/nomebranch

faz o checkout para nomebranch

    git flow release finish (nomebranch)

faz merge da branch **release** pra **MASTER**

cria uma tag para simbolizar o **release** no github

faz merge de volta pra **DEVELOP**

deleta **release** branch e muda para **DEVELOP**

    git flow release publish (nomebranch)

publica branch release no repositorio remoto

### HOTFIX

    git flow hotfix start (nomebranch)

cria uma nova branch baseada na **MASTER**

automaticamente a nomeia como **hotfix**/nomebranch

faz o checkout para nomebranch

    git flow hotfix finish (nomebranch)

faz merge da branch **hotfix** pra **MASTER**

cria uma tag para simbolizar o **hotfix** no github

faz merge da branch **hotfix** na **DEVELOP**

deleta **hotfix** branch e muda para **DEVELOP**

    git flow hotfix publish (nomebranch)

publica branch hotfix no repositorio remoto