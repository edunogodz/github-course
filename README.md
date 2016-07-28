http://try.github.io

git init - Para iniciar a pasta no git
git status - para ver se tem algum arquivo pra ser commitado

git add octocat.txt  - para adicionar um arquivo
git add -A . - 
git reset <filename> para remover algum arquivo

git commit -m "Add cute octocat story" - e um nome pra saber aquele commit

git add '*.txt' - para adicionar todos os arquivo .txt

git commit -m 'Add all the octocat txt files'

git log - para saber o q ja foi comitado
git log --summary  - para ver cada commit

Remote Repositories
git remote add origin https://github.com/try-git/try_git.git

git push -u origin master
git push

git pull origin master - para ver as mudanças no repositorio

git diff HEAD - para ver o q veio de diferente do ultimo commit

git add octofamily/octodog.txt

git diff --staged

git reset octofamily/octodog.txt

git checkout -- octocat.txt - pros arquivos voltarem ao q eram antes

git branch clean_up ´para criar um branch - agora tenho 2 master e clean_up

git checkout clean_up para switch to clean_up

git rm '*.txt' - remover os arquivos

git commit -m "Remove all the cats"

git checkout master

git merge clean_up - para juntar tudo

git branch -d clean_up - para deletar o q vc fez

git push


http://gitreal.codeschool.com/levels/1
git init
git status
git add README.txt

git commit -m "Create a README."

git add --all

git commit -m "Add LICENSE and finish README"

git log

git add <list of files> - add the list of files
git add *.txt
git add docs/*.txt
git add docs/
git add "*.txt"

http://willianjusten.teachable.com/courses/git-e-github-para-iniciantes

git config --list - ver o q tem configurado

mkdir git-course
cd git-course/
git init
ls-la

File Status Lifecycle
Ciclo de vida dos arquivos
Untracked - não marcado e ainda nao foi visto pelo git
(git add)
Unmodified - o file muda para unmodified

Modified - 

Staged - area onde vai ser criada a versão, qdo for criada a versão leva os arquivos

depois do commit volta a ser unmodified

comandos:
git status - para saber como esta as mudanças
criei um arquivo e salvei
o arquivo fica como untracked
git add READM.md
ele coloca o arquivo pra ser comitado

git commit -m "Add Readme.md"

se editar de novo, volta a ser untracked

-Visualizando o Log
git log
git log --decorate
git log --author="edunogodz"
git shortlog
git shortlog sn
git log --graph
git show (e uma hash)

-Visualizando o Diff
git diff - para ver o q foi alterado
git diff --name-only - somente o arquivo modificado

Desvazendo coisas
altera algo salva
ae depois dá
git checkout README.md - q ele volta a versão anterior

git reset HEAD
remover da linha de staged para unstaged

git reset pode ser
--soft - ele vai pegar as modificações e voltar o commit, com o arquivo como unstaged
--mixed- ele vai pegar as modificações e voltar o commit, com o arquivo antes do staged
--hard - vai resetar todo o commit