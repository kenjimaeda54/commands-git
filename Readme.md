### Desfazer

Para retorna um estado anterior do commit voce pode efetuar o git reset ou git revert. </br>
Ideal cenário para reset e momento que ainda não realizou um git push da mudança
Ideal para revert e apos o push

- git reset --soft e o hash do commit que deseja voltar
- git reset tem algumas opções como --soft --hard --mixed , --hard vai voltar e apagar tudo,soft vai voltar o commit anterior manter no stage , mixed mistura dos dois
- git push revert < hash > ex: 343434** --> precisa colocar o hash que quero voltar</br>
- Ele vai criar um novo commit,com os valores anterior apos o revet

##

### Comandos básicos
- git branch --> enxergo as branchs 
- git switch < nome da branch > ex: feat -> para mudar de branch
- git push origin < nome da branch > -d  -> remove a branch remota
- git branch -d < nome da branch >  --> remove a branch local 
- git checkout -b < none branch > ex:feat --> cria uma nova branch
- git checkout -> consigo alternar entre as versões dos arquivos
- git checkout HEAD -- < nome do arquivo > ex: style.css --> consigo voltar ao estado anterior de um arquivo, como também recuperar se ele foi deletado
</br>

##

### Para remover arquivos do stage 

- git rm -r --cached --> <diretório>
- git rm --cached  --> <arquivo>


  
##

### Arvore do github
- git log --decorate  --graph --all --> log com gráfico ideal para enxergar novas mudanças
- git diff --> enxergo todas as alterações do arquivo 
- git diff --name-only --> enxergo apenas os arquivos 
- git diff < nome do arquivo > ex: style.css --> consigo acessar direitamente o arquivo e ver as mudanças 


##

### WorkFlow

- git merge < branch que esta a frente > ex: kenji --> para mergear em uma branch que esta a frente da sua,e so colocar o nome da branch
- git remote -v --> enxergo o link do repositório remoto na maquina
- git remote remove < nome que esta ao lado do link > ex: origin -> removo o repositorio remoto 
- git pull < quem voce esta puxando > ex:origin < para qual branch > ex: master --> se nao deseja referenciar a branch pode apenas colocar git pull 
- git clone < ulr > --> clonar projeto

## Team
Para contribuir com projeto primeiro faz o fork, apos isto, sera feito uma cópia do original no seu repositório remoto, clona esse projeto, trabalha e faz um push com as alterações, apos isto cria um pull request.
</br>

## Edit
- git commit --amend --> para editar o ultimo commit feito,vai abrir no editor seu ultimo commit, dai so renomeiar 
- git update-index --really-refresh ---> caso o git pare de filtrar algo, depois foca adiconar o arquivo usando comando git add --all --v 
- git config --global core.editor code ==> depois fizer git config --global --edit => vai abrir a config do git hub no vscode

## Arquivo não trackeado
- git stash --include-untracked

```git 
[credential]
  helper = osxkeychain

[user]
  name = name user
  email = email user

[core]
  editor = code --wait

[alias]
  c = !git add --all && git commit -m
  s = !git status -s
  l = !git log --pretty=format: '%C(blue)%h%c(red)%d %C(white)%s - %C(cyan)%cn, %C(green)%cr'



```

##

### Para resolver conflitos em branch
- Apos identificar o hash do commit que esta gerando erro , fazer git checkout <hash do commit> 
- Faz um git pull < origin sua branch >  
- Abra seu editor, os codigos que voce criou e os conflitos devem estar marcados 
- Apos aprovar faz um git add .
- Git commit
- Depois retornar a sua branch  e faz uma nova branch com hash do commit, git checkout -b <branch> <hash do commit>  

##
  
### Clonar branch especifica
- git clone -b   < nome da branch > url




