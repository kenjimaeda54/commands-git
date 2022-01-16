
Para retorna um estado anterior do commit voce pode efetuar o git reset ou git revert.
Ideal cenário para reset e momento que ainda nao realizou um git push da mudanca
Ideal para revert e apos o push
git reset --soft e o hash do commit que deseja voltar
git reset tem algumas opções como --soft --hard --mixed , --hard vai voltar e apagar tudo,soft vai voltar o commit anterior manter no stage , mixed mistura dos dois
</br>

**git push revert <hash> ex: 343434** -->  precisa colocar o hash que quero voltar</br>
Ele vai criar um novo commit,com os valores  anterior  apos o revet
</br>

**git branch** --> enxergo a branch atual</br>
**git switch < nome da branch > ex: feat** ->  para mudar de branch</br>

**git checkout -b < none branch > ex:feat** -->  cria uma nova branch</br>
**git checkout** -> consigo alternar entre as versões dos arquivos</br>
**git checkout HEAD -- < nome do arquivo > ex: style.css** --> consigo voltar ao estado anterior de um arquivo, como também recuperar se ele foi deletado</br>
</br>

**git log --decorate --online --graph --all** --> log com gráfico ideal para enxergar novas mudanças</br>
</br>

**git diff** --> enxergo todas as alterações do arquivo </br>
**git diff --name-only** --> enxergo apenas os arquivos </br>
**git diff < nome do arquivo > ex: style.css** --> consigo acessar direitamente o arquivo e ver as mudanças </br>
**git merge < branch que esta a frente > ex: kenji** --> para mergear em uma branch que esta a frente da sua,e so colocar o nome da branch
</br>

**git remote -v** --> enxergo o link do repositório remoto na maquina</br>
**git remote < nome que esta ao lado do link > ex: origin** -> removo o repositorio remoto
