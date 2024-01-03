Oi, aqui é um treinamento do Git e GitHub para versionamento de arquivos para essa plataforma,
a ideia é fazer um treino e saber o que é exatamente a plataforma GitHub e a ferramenta Git.

Tutorial:
É só ir na pasta que você quer enviar para o GitHub, e clique com o botão direito em cima da pasta
que você quer enviar, depois clique com o botão esquerdo em "Open Git Bash here".
Depois na janela que você abriu, é só seguir os seguintes comandos:

gbl_c@DESKTOP-LVVT4I2 MINGW64 ~/OneDrive/Documentos/Projetos/Visual Studio Code/Projeto1
$ git init
Initialized empty Git repository in C:/Users/gbl_c/OneDrive/Documentos/Projetos/Visual Studio Code/Projeto1/.git/

gbl_c@DESKTOP-LVVT4I2 MINGW64 ~/OneDrive/Documentos/Projetos/Visual Studio Code/Projeto1 (master)
$ git add Readme.md
## Adiciona apenas o arquivo especificado ##

gbl_c@DESKTOP-LVVT4I2 MINGW64 ~/OneDrive/Documentos/Projetos/Visual Studio Code/Projeto1 (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   Readme.md


gbl_c@DESKTOP-LVVT4I2 MINGW64 ~/OneDrive/Documentos/Projetos/Visual Studio Code/Projeto1 (master)
$ git commit -m "first commit"
[master (root-commit) 5e6014b] first commit
 1 file changed, 2 insertions(+)
 create mode 100644 Readme.md

gbl_c@DESKTOP-LVVT4I2 MINGW64 ~/OneDrive/Documentos/Projetos/Visual Studio Code/Projeto1 (master)
$ git status
On branch master
nothing to commit, working tree clean

gbl_c@DESKTOP-LVVT4I2 MINGW64 ~/OneDrive/Documentos/Projetos/Visual Studio Code/Projeto1 (master)
$ git branch -M "main"

gbl_c@DESKTOP-LVVT4I2 MINGW64 ~/OneDrive/Documentos/Projetos/Visual Studio Code/Projeto1 (main)
$ git remote add origin https://github.com/GBLONE/ProjectGit.git

gbl_c@DESKTOP-LVVT4I2 MINGW64 ~/OneDrive/Documentos/Projetos/Visual Studio Code/Projeto1 (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 342 bytes | 171.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/GBLONE/ProjectGit.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

Aqui você subiu tudo o que precisava, mas e se eu precisar subir mais alguma coisa?
Como faria se caso meu projeto tivesse que subir mais arquivos e atualizar os arquivos
existentes? 
Na mesma janela do "Open Git Bash here" você irá escrever e seguir os seguintes comandos:

gbl_c@DESKTOP-LVVT4I2 MINGW64 ~/OneDrive/Documentos/Projetos/Visual Studio Code/Projeto1 (main)
$ git add . 
## O ponto adiciona todos os arquivos do diretório/pasta que você indicou antes ##

gbl_c@DESKTOP-LVVT4I2 MINGW64 ~/OneDrive/Documentos/Projetos/Visual Studio Code/Projeto1 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   Readme.md
        new file:   index.html
        new file:   kmeans graphic 1.png
        new file:   kmeans graphic 2.png
        new file:   kmeans.png
        new file:   matplotlibFigura1.png
        new file:   matplotlibFigura2.png

gbl_c@DESKTOP-LVVT4I2 MINGW64 ~/OneDrive/Documentos/Projetos/Visual Studio Code/Projeto1 (main)
$ git commit -m "criacaoProjeto"
[main 23acf9b] criacaoProjeto
 7 files changed, 77 insertions(+), 1 deletion(-)
 create mode 100644 index.html
 create mode 100644 kmeans graphic 1.png
 create mode 100644 kmeans graphic 2.png
 create mode 100644 kmeans.png
 create mode 100644 matplotlibFigura1.png
 create mode 100644 matplotlibFigura2.png

gbl_c@DESKTOP-LVVT4I2 MINGW64 ~/OneDrive/Documentos/Projetos/Visual Studio Code/Projeto1 (main)
$ git push origin main
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 4 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (9/9), 257.17 KiB | 19.78 MiB/s, done.
Total 9 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/GBLONE/ProjectGit.git
   5e6014b..23acf9b  main -> main

Como pode ver não precisa mais colocar o git remote add origin "linkDoSeuProjeto",
por que você está na mesma janela e já está com o git remote nessa pasta "ligado" ao
GitHub. 