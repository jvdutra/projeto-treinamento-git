# Iniciais
    git init
        comando para iniciar o repositorio
    git add .
        adiciona todos os arquivos nao trackeados (untracked) no stage, onde aguardam o commit
            o . passa todos os arquivos, arquivos podem tbm ser passados individualmente
    git commit -m "mensagem"
        realiza um commit para salvar alterações com uma mensagem que pode ser definida
    git push
        envia todos os commit para o repositorio remoto, no github
    git pull
        puxa arquivos do repositorio remoto, usado pra sincronizar com arquivos
    git status
        mostra status de arquivos

# Branches
    git branch 
        lista todas as branchs do projeto
    git branch (nomebranch)
        cria uma branch
    git checkout (nomebranch)
        altera a branch atual
    git checkout -b (nomebranch)
        cria uma branch e a define como branch atual
    git branch -d (nomebranch)
        deletar branch
    git merge (nomebranch)
        faz merge da branch atual com a branch indicada
    git stash
        guarda todas as alterações não commitadas
    git stash list
        lista todos as alterações na stash
    git stash apply (index)
        recupera alterações, se não passar o indice recupera a mais recente
    git stash pop
        recupera e remove do stash
    git stash drop
        remove do stash
    