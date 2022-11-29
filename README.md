# testgitdotnet

mkdir testgitdotnet
cd .\testgitdotnet\
dotnet new console

git init

git remote add github https://github.com/albertogallen/testgitdotnet.git
git fetch
git pull github main
code .

editar .gitignore
.vs
.vscode
bin
obj

git add .
git commit -m "first dotnet"
git push --set-upstream github master

documentar
git add .
git commit -m "doc"
git push github

--- 
error
como no he dicho rama remota en el push 
ha subido la rama de master del local al remoto "github" creando una rama nueva en remoto teniendo dos la master y la main

git checkout main
git rebase master
git push github main

git checkout master


git branch -d main

 git push github
 git push github :main
 
 lo mismo
 git push github --delete main
 da error por que es la rama por defecto en remoto
 si la borro en la web ya puedo elimnar la rama remota
