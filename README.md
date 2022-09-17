<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=94d355&height=120&section=header"/>



[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=94d355&size=35&center=true&vCenter=true&width=1000&lines=Be+Welcome!;pegue+o+café+e+bora+para+o+código+:%29)](https://git.io/typing-svg)

<p align="center" >Espero ajudar todos os iniciantes em git com esse pequeno glossário.</p>
<p align="center" >
    <img width="300" src="./assets/giphy.gif" >
</p>

## Explicando cada processo dos comandos git para criar um repositório:

Commands                                     | Description
---------------------------------------------|-------------------------------------------------------------
`git init`                                   | inicia um repositório git vazio
`git add (nome do arquivo)`                  | manda os arquivos pra area de standing
`git status`                                 | (opcional) mostra o status para verificar o estado da branch
`git commit -m "primeiro commit"`            | gerando commit
`git status`                                 | (opcional) mostra o status para verificar o estado da branch
`git branch -m "main"`                       | renomeando a branch padrão
`git remote add origin (link do repositório)`| conecta o repositório remoto com o git local
`git push -u orgin main`                     | empurra os commit's do repositório local-(git) para o repositório remoto-(github)

## alterando e adicionando arquivos:

Commands                            | Description
------------------------------------|-------------------------------------------------------
`git add .`                         | adiciona todas as alterações
`git commit -m "criação do projeto"`| commitando
`git push origin main`              | mandando a alteranção para o repositório remoto/github

(observação: não precisa do "-u" no comando poís só se usa na primeira vez que cria o repositório)

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

## Clonando repositório:

Commands                                                 | Description
---------------------------------------------------------|--------------------------------------
`git clone https://github.com/user/nomeDorepositorio.git`| clona um repositório especificando um link de repositório

## Clonando repositório criando branch nova e adicionando alterações:
(observação: essa forma so é possível se você tiver acesso de colaborador ao repositório que esta clonando, caso não tiver o acesso de colaborador não será capaz de fazer alterações)

    Exemplo:
    Caso você e seu colega queiram levantar um projeto utilizando o mesmo repositório
    Vocês teram que seguir os seguintes passos:
    1 - A Pessoa que quer dar o acesso de colaborador terá que acessar as configurações do repositório
    2 - Depois acessar (Collaborators/Colaboradores) logo em seguida (add people/adicionar pessoas)
    3 - Pesquisa pelo nome de User do seu colega e adiciona ele e pronto você estará apto a seguir esses passos
    Para contribuir ao repositório

Commands                                                 | Description
---------------------------------------------------------|--------------------------------------
`git clone https://github.com/user/nomeDoRepositorio.git`| clona um repositório especificando um link de repositório
`git checkout -b "novo-botao"`                           | criando nova branch
`git add .`                                              | adicionado arquivos a ela
`git commit -m "novo-botao"`                             | commitando
`git push origin novo-botao`                             | empurrando as alterações para a branch criada

## Atualizando arquivos do git(local):

Commands                                                 | Description
---------------------------------------------------------|--------------------------------------
`git pull`                                               | usado para buscar e baixar conteúdo de repositórios remotos e fazer a atualização imediata ao repositório local para que os conteúdos sejam iguais

## Juntando ramificações/branch:

Commands              | Description
--------------------- |------------------------------------------------------
`git checkout main`   | voltando para branch main
`git merge novo-botao`| juntando com outra branch
`git push orgin main` | empurrando as alterações no repositório remoto/github

## Revertando burrada com commit:

Commands                          | Description
----------------------------------|-------------------------------------------------------
`git log`                         | mostra todos os commits
`git reflog`                      | mostra todos os commits e seus identificadores
`git reset --hard (identificador)`| volta para o commit passando o identificador referente

## Adicionando arquivos ao um commit já feito:

Commands                                        | Description
------------------------------------------------|---------------------------
`git add (arquivo que quer adicionar no commit)`|
`git commit --amend --no-edit`                  | adiciona arquivo no commit

## Verificando arquivos dentro de uma branch:

Commands                                         | Description
-------------------------------------------------|---------------------------------------
`git log`                                        | para ver todos as branch's e seus id's
`git show --pretty="" --name-only (id da branch)`| mostra todos arquivos dentro da branch especificada

## Removendo arquivo especifico depois de ter adicionado:

Commands                             | Description
-------------------------------------|----------------------------------
`git status`                         | mostra as alterações commitadas
`git restore --staged meuarquivo.txt`| remove o arquivo especificado
`git status`                         | mostra que o arquivo foi removido

## Processos sem explicação:

    echo "# ProjetoGit" >> README.md
    git init
    git add README.md
    git commit -m "first commit"
    git branch -M main
    git remote add origin https://github.com/seuUserName/nomeDorepositorio.git
    git push -u origin main

<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=94d355&height=120&section=footer"/>