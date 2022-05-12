## GitHub. HW_2
#### 1. На локальном репозитории сделать ветки для:  
- Postman  
- Jmeter  
- CheckLists  
- Bag Reports  
- SQL  
- Charles  
- Mobile testing  
  
```
git clone https://github.com/marg0sh/GitHub.git
cd GitHub

git branch BugReports
git branch Charles
git branch CheckLists
git branch Jmeter
git branch Mobile_Testing
git branch Postman
git branch SQL
```
  
#### 2. Запушить все ветки на внешний репозиторий  
```
git push -u origin BugReports
git push -u origin Charles
git push -u origin CheckLists
git push -u origin Jmeter
git push -u origin Mobile_Testing
git push -u origin Postman
git push -u origin SQL
```
*или*  
```
git push -u origin --all
```
  
#### 3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта  
```
git checkout BugReports
vim BugReports.txt
```
*режим редактирования - i*   
```
ID
Summary
Description
Actual result
Expected result
Attachments
Priority
Severity
Status

```
*выйти из режима редактирования с сохранением - Esc :wq Enter*   
```
git add .; git commit -m 'add BugReports.txt'
```
  
#### 4. Запушить структуру багрепорта на внешний репозиторий  
```
git checkout main
git push -u origin BugReports
```
  
#### 5. Вмержить ветку Bag Reports в Main  
```
git merge BugReports
```
  
#### 6. Запушить main на внешний репозиторий.  
```
git push
```
  
#### 7. В ветке CheckLists набросать структуру чек листа.  
```
git checkout CheckLists
vim CheckLists.txt
```
*режим редактирования - i*  
```
Name
Status

```
*выйти из режима редактирования с сохранением - Esc :wq Enter*   
```
git add .; git commit -m 'add CheckLists.txt'
```
  
#### 8. Запушить структуру на внешний репозиторий  
```
git checkout main
git push -u origin CheckLists
```
  
#### 9. На внешнем репозитории сделать Pull Request ветки CheckLists в main    
*Pull requests  
CheckLists  
Compare & pull request  
Create pull request  
Merge pull request  
Confirm merge*  

#### 10. Синхронизировать Внешнюю и Локальную ветки Main  
```
git fetch
git pull
```
