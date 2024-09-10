## GIT FLOW

Git flow é uma ferramenta que facilita os comandos de criação e manipulação de branches, encurtando os comandos.

## comandos iniciais

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