~~~Com explicação
# Lista de processos do git

## Explicando cada processo dos comandos git para criar um repositorio:

Commands                                     | Description
---------------------------------------------|-------------------------------------------------------------
`git init`                                   | inicia um repositorio git vazio
`git add (nome do arquivo)`                  | manda os arquivos pra area de standing
`git status`                                 | (opcional) mostra o status para verificar o estado da branch
`git commit -m "primeiro commit"`            | gerando commit
`git status`                                 | (opcional) mostra o status para verificar o estado da branch
`git branch -m "main"`                       | renomeando a padrão branch
`git remote add origin (link do repositorio)`| linka o repositorio remoto com o git local
`git push -u orgin main`                     | empurra os commit's do repositorio local-(git) para o repositorio remoto-(github)

## alterando e adicionando arquivos:

Commands                            | Description
------------------------------------|-------------------------------------------------------
`git add .`                         | adiciona todas as alterações
`git commit -m "criação do projeto"`| commitando
`git push origin main`              | mandando a alteranção para o repositorio remoto/github

(observaçõa não precisa do "-u" no comando poís só se usa na primeira vez que cria o repositorio)

## Criando uma ramificação/branch nova e adicionando novos arquivos:

Commands                      | Description
------------------------------|----------------------------------------------
`git checkout -b "novo-botao"`| criando nova branch
`git add .`                   | adicionado arquivos a ela
`git commit -m "novo-botao"`  | commitando
`git push origin novo-botao`  | empurrando as alterações para a branch criada

## Voltando para branch's:	

Commands                                  | Description
------------------------------------------|--------------------------------------
`git checkout main`                       | voltando para ramificação/branch main
`git checkout NomeDaBranchExistenteCriada`| voltando para outra branch

## Juntando ramificações/branch:

Commands              | Description
--------------------- |------------------------------------------------------
`git checkout main`   | voltando para branch main
`git merge novo-botao`| juntando com outra branch
`git push orgin main` | empurrando as alterações no repositorio remoto/github

## Processos sem explicação:

    echo "# ProjetoGit" >> README.md
    git init
    git add README.md
    git commit -m "first commit"
    git branch -M main
    git remote add origin https://github.com/jonasmarquesdev/nomedorepositorio.git
    git push -u origin main

## Revertando burrada com commit:

Commands                          | Description
----------------------------------|-------------------------------------------------------
`git log`                         | printa todos os commits
`git reflog`                      | printa todos os commits e seus identificadores
`git reset --hard (identificador)`| volta para o commit passando o identificador referente

## Adicionando arquivos ao um commit já feito:

Commands                                        |
------------------------------------------------|
`git add (arquivo que quer adicionar no commit)`|
`git commit --amend --no-edit`                  |

## Verificando arquivos dentro de uma branch:

Commands                                         | Description
-------------------------------------------------|---------------------------------------
`git log`                                        | para ver todos as branch's e seus id's
`git show --pretty="" --name-only (id da branch)`|

## Removendo arquivo especifico depois de ter adicionado:

Commands                             | Description
-------------------------------------|----------------------------------
`git status`                         | Mostra as alterações commitadas
`git restore --staged meuarquivo.txt`|
`git status`                         | Mostra que o arquivo foi removido
~~~
~~~Sem explicação
## Processos sem explicação:

    echo "# ProjetoGit" >> README.md
    git init
    git add README.md
    git commit -m "first commit"
    git branch -M main
    git remote add origin https://github.com/jonasmarquesdev/nomedorepositorio.git
    git push -u origin main
~~~