
Para retonar um estado anterior do commit voce pode efetuar o git reset e git revert.


Ideal cenario para  reset e momento que ainda nao realizou um git push da mudanca
Ideial para revert e apos o push 
git reset --soft e o hash do commit que deseja voltar 
git reset tem algumas opcoes como --soft --hard --mixed ,  --hard vai voltar e apagar tudo,soft vai voltar o commit anteior  manter  no stage , mixed mistura dos dois


git branch --> enchergo a branch atual

git switch <nome da branch> para mudar de branch
git checkout -b <none branch> cria uma nova branch


log com grafico ideal para enchergar novas mudancas 
git log --decorate --oneline --graph --all


