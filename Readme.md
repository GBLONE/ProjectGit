Oi, aqui é um treinamento do Git e GitHub para versionamento de arquivos para essa plataforma,
a ideía é fazer um treino e saber o que é exatamente a plataforma GitHub e a ferramenta Git.

Tutorial:
É só ir na pasta que você quer enviar para o GitHub, e clique com o botão direito em cima da pasta
que você quer enviar, depois clique com o botão esquerdo em "Open Git Bash here".
Depois é só seguir os seguintes comandos:

gbl_c@DESKTOP-LVVT4I2 MINGW64 ~/OneDrive/Documentos/Projetos/Visual Studio Code/Projeto1
$ git init
Initialized empty Git repository in C:/Users/gbl_c/OneDrive/Documentos/Projetos/Visual Studio Code/Projeto1/.git/

gbl_c@DESKTOP-LVVT4I2 MINGW64 ~/OneDrive/Documentos/Projetos/Visual Studio Code/Projeto1 (master)
$ git add Readme.md

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
