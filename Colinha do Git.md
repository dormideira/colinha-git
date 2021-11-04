# Conteúdo

## Criação

1. Copiar repositório
`git clone https://repositoriox.git`

1. Novo repositório local 
`git init`

## Branches 

1. Listar todas as branches existentes
`git branch -av`

1. Mudar branch HEAD
`git checkout <branch>`

1. Nova branch com base
`git checkout --track <remote/branch>`

1. Deletar uma branch local
`git branch -d <branch>`

1. Marcar o commit atual com uma tag
`git tag <tag-name>`

## Mudanças locais

1. Arquivos alterados em seu diretório de trabalho
`git status`

1. Mudanças em arquivos rastreados
`git diff`

1. Adicionar todas as mudanças atuais no próximo commit
`git add .`

1. Adicionar algumas mudanças no <arquivo> para o próximo commit
`git add . -p <arquivo>`

1. Dar commit em todas as alterações locais em arquivos rastreados
`git commit -a`

1. Dar commit em alterações já preparadas
`git commit`

1. Mudar o último commit
`git commit --amend`

## Histórico

1. Mostrar todos os commits, começando pelo mais novo
`git log`

1. Mostrar mudanças em um <arquivo> ao longo do tempo
`git log -p <arquivo>`

1. Mostrar quem alterou o que e quando no <arquivo>
`git blame <arquivo>`

## Remoto, pull e push

1. Listar todos os repositórios remotos configurados atualmente
`git remote -v`

1. Mostrar informações sobre o repositório <remoto>
`git remote show <remoto>`

1. Adicionar um novo repositório remoto chamado <remoto>
`git remote add <remoto> <url>`

1. Baixar todas as alterações de <remoto> sem integrar no HEAD
`git fetch <remoto>`

1. Baixar todas as alterações de <remoto> e integrar diretamente no HEAD
`git pull <remoto> <branch>`

1. Excluir uma branch do repositório remoto
`git branch -dh <remoto/branch>`

1. Publicar tags
`git push --tags`

## Merge e rebase

1. Dar merge da <branch> no HEAD atual
`git merge <branch>`

1. Fazer rebase do HEAD atual na <branch>
`git rebase <branch>`

1. Abortar um rebase
`git rebase --abort`

1. Continuar rebase depois de resolver conflitos
`git rebase --continue`

1. Usar a ferramenta de merge para resolver conflitos
`git mergetool`

1. Usar o editor para resolver conflitos manualmente e marcar o arquivo como resolvido depois de resolver
`git add <arquivo-resolvido>`
`git rm <arquivo-resolvido>`

## Desfazer

1. Descartar mudanças locais no diretório de trabalho
`git reset -hard HEAD`

1. Descartar alterações locais para <arquivo>
`git checkout HEAD <file>`

1. Reverter um commit (criando um novo commit com mudanças contrárias)
`git revert <commit>`

1. Redefinir o HEAD para um commit anterior... 

    1. ... descartando todas as alterações desde então
`git reset -hard <commit>`

    1. ... mantendo todas as mudanças como não-planejadas
`git reset <commit>`

    1. ... mantendo as mudanças locais que ainda não foram para um commit
`git reset -keep <commit>`

## Referência

Transcrito da imagem feita por Odemir Depieri Jr. <https://www.linkedin.com/in/odemir-depieri-jr?miniProfileUrn=urn%3Ali%3Afs_miniProfile%3AACoAABq3R1EBa2aUYMmKarZriOlFD2JSUhvAvls&lipi=urn%3Ali%3Apage%3Ad_flagship3_feed%3BnsFU2U6JRwWsDYsfCnIGSQ%3D%3D&licu=urn%3Ali%3Acontrol%3Ad_flagship3_feed-actor_container&lici=kawngAoqon5Kk4OKvJ8Vlw%3D%3D>, acessado em 03/11/2021. 

## Tudo em uma tabela só

| Tópico | Ação | Comando |
| --- | --- | --- |
| Criação | Copiar repositório | `git clone https://repositoriox.git` |
| Criação | Novo repositório local | `git init` |
| Branches | Listar todos os branches existentes | `git branch -av` |
| Branches | Mudar branch HEAD | `git checkout <branch>` |
| Branches | Nova branch com base | `git checkout --track <remote/branch>` |
| Branches | Deletar uma branch local | `git branch -d <branch>` |
| Branches | Marcar o commit atual com uma tag | `git tag <tag-name>` |
| Mudanças locais | Arquivos alterados em seu diretório de trabalho | `git status` |
| Mudanças locais | Mudanças em arquivos rastreados | `git diff` |
| Mudanças locais | Adicionar todas as mudanças atuais no próximo commit | `git add .` |
| Mudanças locais | Adicionar algumas mudanças no <arquivo> para o próximo commit | `git add . -p <arquivo>` |
| Mudanças locais | Dar commit em todas as alterações locais em arquivos rastreados | `git commit -a` |
| Mudanças locais | Dar commit em alterações já preparadas | `git commit` |
| Mudanças locais | Mudar o último commit | `git commit --amend` |
| Histórico | Mostrar todos os commits, começando pelo mais novo | `git log -p <arquivo>` |
| Histórico | Mostrar mudanças em um <arquivo> ao longo do tempo | `git blame <arquivo>` |
| Histórico | Mostrar quem alterou o que e quando no <arquivo> | `git remote -v` |
| Atualização e push | Listar todos os repositórios remotos configurados atualmente | `git remote add <remote> <url>` |
| Atualização e push | Mostrar informações sobre o repositório <remoto> | `git remote show <remoto>` |
| Atualização e push | Adicionar um novo repositório remoto chamado <remoto> | `git remote add <remoto> <url>` |
| Atualização e push | Baixar todas as alterações de <remoto> sem integrar no HEAD | `git fetch <remoto>` |
| Atualização e push | Baixar todas as alterações de <remoto> e integrar diretamente no HEAD | `git pull <remoto> <branch>` |
| Atualização e push | Excluir uma branch do repositório remoto | `git branch -dh <remoto/branch>` |
| Atualização e push | Publicar tags | `git push --tags` |
| Merge e rebase | Dar merge do <branch> no HEAD atual | `git merge <branch>` |
| Merge e rebase | Fazer rebase do HEAD atual na <branch> | `git rebase <branch>` |
| Merge e rebase | Abortar um rebase | `git rebase --abort` |
| Merge e rebase | Continuar rebase depois de resolver conflitos | `git rebase --continue` |
| Merge e rebase | Usar a ferramenta de merge para resolver conflitos | `git mergetool` |
"| Merge e rebase | Usar o editor para resolver conflitos manualmente e marcar o arquivo como resolvido depois de resolver | `git add <arquivo-resolvido>`
`git rm <arquivo-resolvido>` |"
| Desfazer | Descartar mudanças locais no diretório de trabalho | `git reset -hard HEAD` |
| Desfazer | Descartar alterações locais para <arquivo> | `git checkout HEAD <file>` |
| Desfazer | Reverter um commit (criando um novo commit com mudanças contrárias) | `git revert <commit>` |
| Desfazer | Redefinir o HEAD para um commit anterior...  |  |
| Desfazer | ... descartando todas as alterações desde então | `git reset -hard <commit>` |
| Desfazer | ... mantendo todas as mudanças como não-planejadas | `git reset <commit>` |
| Desfazer | ... mantendo as mudanças locais que ainda não foram para um commit | `git reset -keep <commit>` |
