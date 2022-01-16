
Para retonar um estado anterior do commit voce pode efetuar o git reset ou git revert.
Ideal cenario para  reset e momento que ainda nao realizou um git push da mudanca
Ideial para revert e apos o push 
git reset --soft e o hash do commit que deseja voltar 
git reset tem algumas opcoes como --soft --hard --mixed ,  --hard vai voltar e apagar tudo,soft vai voltar o commit anteior  manter  no stage , mixed mistura dos dois

</br>
git push revert <hash> ex: 343434, precisa colocar  o hash que quero voltar
Ele vai criar um novo comit,neste novo commit vai possuir os valores dos historico  anterior apos o revet 

</br>
git branch --> enchergo a branch atual
git switch <nome da branch> ex: feat,para mudar de branch
</br>
git checkout -b <none branch> ex:feat,cria uma nova branch
git checkout -> consigo alterar entre as versoes dos arquivos e possivel ate voltaer um arquivo especifico
**git checkout HEAD -- {nome do arquivo} ex: style.css**
</br>

log com grafico ideal para enchergar novas mudancas 
**git log --decorate --oneline --graph --all**

</br>
git diff --> enchergo todas as alteracoes do arquivo
git diff --name-only --> enchergo apenas os arquivos
git diff {nome do arquivo} ex: style.css,consigo acessar direatamente o arquivo e ver as mudancas
</br>
 git merge {branch que esta a frente} ex: kenji,para mergear em uma branch que esta a frente da sua,fique na sua e coloque o nome da branch
</br>
 **git remote -v** --> enchergo o link do repositorio remoto na maquina
`git remote {nome que esta ao lado do link} ex: origin` -> removo o repositorio remoto

