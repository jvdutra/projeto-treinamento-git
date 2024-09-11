## GIT FLOW

Git flow é uma ferramenta que facilita os comandos de criação e manipulação de branches, encurtando os comandos.

## comandos iniciais
### FEATURE

    git flow feature start (nomebranch)

cria uma nova branch baseada na develop
automaticamente a nomeia como feature/nomebranch
faz o checkout para nomebranch

    git flow feature finish (nomebranch)

faz merge da feature/nomebranch na develop
deleta a feature/nomebranch
muda para a develop

    git flow feature publish (nomebranch)

cria uma branch remota

### RELEASE

    git flow release start (nomebranch)

cria uma nova branch baseada na develop
automaticamente a nomeia como release/nomebranch
faz o checkout para nomebranch

    git flow release finish (nomebranch)

faz merge da branch release pra master
cria uma tag para simbolizar o release no github
faz merge de volta pra develop
deleta release nomebranch e muda branch atual pra develop

    git flow release publish (nomebranch)

cria uma branch remota

### HOTFIX

    git flow hotfix start (nomebranch)

cria uma nova branch baseada na develop
automaticamente a nomeia como hotfix/nomebranch
faz o checkout para nomebranch

    git flow hotfix finish (nomebranch)

faz merge da branch hotfix pra master
cria uma tag para simbolizar o hotfix no github
faz merge da branch hotfix na develop
deleta hotfix branch e muda para develop

    git flow hotfix publish (nomebranch)

cria branch remota no repositorio