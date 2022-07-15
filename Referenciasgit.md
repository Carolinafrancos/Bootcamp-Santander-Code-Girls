# Anotações sobre GIT

$ git init: Iniciando um Repositório
$ rm -rf .git: Apagando um repositório

$ git status: Listando Arquivos Modificados
 git checkout . : Desfazendo Alterações
 git reset : Removendo arquivos do Stage
 git revert HEAD : Desfazendo o último commit
$ git commit --amend : Renomear Commit
$ git branch : Listando Branches
$ git checkout minha-branch : Indo para outra branch
git branch -d nome-da-branch : Excluindo branches
git branch -m novo-nome-da-branch : Renomeando branches

          i---j---k     <== branch 'minha branch'
         /
a---b---c---d---h---l   <== branch 'main'
     \         /
      e---f---g         <== branch 'minha outra branch'
	  
1---2---3---4			<== branch `órfã`  : Branch Órfã

$ git log : Visualizando o Histórico de Commits

//deixar o comando disponível apenas no repositório atual
git config alias.dog "log --all --decorate --oneline --graph"
//deixar o comando global em sua máquina, ficando disponível para qualquer repositório
git config --global alias.dog "log --all --decorate --oneline --graph"  : Criando atalhos personalizados