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
