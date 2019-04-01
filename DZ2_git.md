Работа с GIT
1) Создать новый репозиторий на сайте github
Education-practice
2) iTerm клонировать себе репозиторий
git clone ссылка_с_github
*ругается, что репозиторий пустой, но клонирует*
3) Создать файл README на сайте, отредактировать из атома
4) Создать файлы из терминала
(сначала надо перейти в локальный репозиторий)
➜  ~ cd Education-practice
touch DZ1_nginx.md
touch DZ2_git.md
<!-- попробовать вместо touch - cat or echo -->
<!-- найти как переименовать созданные файлы -->
5) Забыла создать ветку. Создать ветку
~ git branch Edu_1.0
6) Поредактировала с помощью cat файлы .md
7) Подготовить файлы к коммиту
 Education-practice git:(Edu_1.0) ✗ git add DZ1_nginx.md DZ2_git.md README.md
прверила статус:
➜  Education-practice git:(Edu_1.0) ✗ git status
совершила коммит
➜  Education-practice git:(Edu_1.0) ✗ git commit -m "new branch and sorting log"
попыталась закинуть коммит на сервер
➜  Education-practice git:(Edu_1.0) git push
fatal: The current branch Edu_1.0 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin Edu_1.0
*получила по жопе, т.к. на гитхабе нет ветки Edu_1.0, подсказка: git push --set-upstream origin Edu_1.0*
закинула:
➜  Education-practice git:(Edu_1.0) git push --set-upstream origin Edu_1.0
Counting objects: 5, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 1.90 KiB | 1.90 MiB/s, done.
Total 5 (delta 0), reused 0 (delta 0)
remote:
remote: Create a pull request for 'Edu_1.0' on GitHub by visiting:
remote:      https://github.com/styazhkina/Education-practice/pull/new/Edu_1.0
remote:
To github.com:styazhkina/Education-practice.git
 * [new branch]      Edu_1.0 -> Edu_1.0
Branch 'Edu_1.0' set up to track remote branch 'Edu_1.0' from 'origin'.
8) Этот файл еще не кидала на сервер
