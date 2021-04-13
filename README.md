# Prueba
PS C:\Users\Uy2021\Desktop\Clases Zoom\Practica> git add .
PS C:\Users\Uy2021\Desktop\Clases Zoom\Practica> git commit -m "error con la fuente sin solucionar"
[master 4c7c36e] error con la fuente sin solucionar
 1 file changed, 1 insertion(+), 1 deletion(-)
PS C:\Users\Uy2021\Desktop\Clases Zoom\Practica> git add .
PS C:\Users\Uy2021\Desktop\Clases Zoom\Practica> git commit -m "sigue el error"
 1 file changed, 1 insertion(+), 1 deletion(-)
PS C:\Users\Uy2021\Desktop\Clases Zoom\Practica> push origin master
push : El término 'push' no se reconoce como nombre de un cmdlet, función, archivo de script o programa ejecutable. Compruebe si escribió         
correctamente el nombre o, si incluyó una ruta de acceso, compruebe que dicha ruta es correcta e inténtelo de nuevo.
En línea: 1 Carácter: 1
+ push origin master
+ ~~~~
    + CategoryInfo          : ObjectNotFound: (push:String) [], CommandNotFoundException
PS C:\Users\Uy2021\Desktop\Clases Zoom\Practica> git push origin master
To https://github.com/LeanArbelo22/Prueba.git
 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'https://github.com/LeanArbelo22/Prueba.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
PS C:\Users\Uy2021\Desktop\Clases Zoom\Practica> git push --help
PS C:\Users\Uy2021\Desktop\Clases Zoom\Practica> git push origin master
To https://github.com/LeanArbelo22/Prueba.git
 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'https://github.com/LeanArbelo22/Prueba.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\Uy2021\Desktop\Clases Zoom\Practica> git pull <remote> master:dev
En línea: 1 Carácter: 10
+ git pull <remote> master:dev
El operador '<' está reservado para uso futuro.
    + CategoryInfo          : ParserError: (:) [], ParentContainsErrorRecordException
    + FullyQualifiedErrorId : RedirectionNotSupported
 
PS C:\Users\Uy2021\Desktop\Clases Zoom\Practica> git pull remote master:dev
fatal: 'remote' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
PS C:\Users\Uy2021\Desktop\Clases Zoom\Practica> git remote name
error: Unknown subcommand: name
usage: git remote [-v | --verbose]
   or: git remote add [-t <branch>] [-m <master>] [-f] [--tags | --no-tags] [--mirror=<fetch|push>] <name> <url>
   or: git remote rename <old> <new>
   or: git remote remove <name>
   or: git remote set-head <name> (-a | --auto | -d | --delete | <branch>)
   or: git remote prune [-n | --dry-run] <name>
   or: git remote [-v | --verbose] update [-p | --prune] [(<group> | <remote>)...]
   or: git remote get-url [--push] [--all] <name>
   or: git remote set-url --add <name> <newurl>

    -v, --verbose         be verbose; must be placed before a subcommand

PS C:\Users\Uy2021\Desktop\Clases Zoom\Practica> git remote rename
usage: git remote rename <old> <new>

PS C:\Users\Uy2021\Desktop\Clases Zoom\Practica> git remote add origin https://github.com/LeanArbelo22
error: remote origin already exists.
PS C:\Users\Uy2021\Desktop\Clases Zoom\Practica> git https://github.com/LeanArbelo22 rename
git: 'https://github.com/LeanArbelo22' is not a git command. See 'git --help'.
PS C:\Users\Uy2021\Desktop\Clases Zoom\Practica> git pull https://github.com/LeanArbelo22/Prueba.git master:dev
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 2.72 KiB | 16.00 KiB/s, done.
From https://github.com/LeanArbelo22/Prueba
 Index.html => index.html | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)
 rename Index.html => index.html (99%)
PS C:\Users\Uy2021\Desktop\Clases Zoom\Practica> git add .
PS C:\Users\Uy2021\Desktop\Clases Zoom\Practica> git commit -m "solucionado error failed to push some refs to 'https://github.com/LeanArbelo22/Prueba.git'
>> hint: Updates were rejected because the remote contains work that you do
>> hint: not have locally. This is usually caused by another repository pushing
>> hint: (e.g., 'git pull ...') before pushing again.
>> hint: See the 'Note about fast-forwards' in 'git push --help' for details. por el cambio de nombre de index en mayuscula a miniscula, git pull 
{remote} (enlace de repositorio) master:dev"
On branch master
Your branch is ahead of 'origin/master' by 4 commits.
  (use "git push" to publish your local commits)
