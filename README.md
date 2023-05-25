<h1 align="center">Git branching homework</h1>

1. На локальном репозитории сделать ветки для:
```
- Postman
- Jmeter
- CheckLists
- Bug Reports
- SQL
- Charles
- Mobile testing
```
_Создание одной ветки_ - `git branch <branch_name>`, _создание всех веток одной командой_ - `git branch Postman && git branch Jmeter && git branch CheckLists && git branch Bug_Reports && git branch SQL && git branch Charles && git branch Mobile_testing`

2. Запушить все ветки на внешний репозиторий - `git push -u origin --all`, `-u` - _опция, которая позволяет отслеживать ссылку на удаленную ветку,_ `--all` - _данная опция позволяет запушить все ветки сразу._
3. В ветке Bug Reports сделать текстовый документ со структурой баг репорта - `git checkout Bug_Reports` > `vim bug_report.txt`
4. Запушить структуру багрепорта на внешний репозиторий - `git add . && git commit -m 'added bug report' && git push`
5. Вмержить ветку Bag Reports в Main - `git checkout main` > `git merge Bug_Reports`
6. Запушить main на внешний репозиторий - `git push`
7. В ветке CheckLists набросать структуру чек листа - `git checkout CheckLists` > `vim checklist.txt`
8. Запушить структуру на внешний репозиторий - `git add . && git commit -m 'added checklist' && git push`
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main:
- _Находясь в удалённом репозитории выбрать ветку - Checklists,_  
- _При нажатии на кнопку "Compare & pull request" - открывается интерфейс pull request,_  
- _Указать коммит в первой форме,_  
- _Нажать "Create pull request",_  
- _После этого на странице слияния нажать на кнопки - "Merge pull request" и "Confirm merge"_  
10. Синхронизировать Внешнюю и Локальную ветки Main - `git pull`
