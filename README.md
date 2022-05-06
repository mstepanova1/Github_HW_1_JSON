# Git_HW_1_JSON

1. Создать внешний репозиторий c названием JSON
https://github.com/mstepanova1/Git_HW_1_JSON.git

 2. Клонировать репозиторий JSON на локальный компьютер
git clone https://github.com/mstepanova1/Git_HW_1_JSON.git

 3. Внутри локального JSON создать файл “new.json”
cd Git_HW_1_JSON
touch new.json

 4. Добавить файл под гит
git add new.json

 5. Закоммитить файлJo"
git commit -m "add new.json"

 6. Отправить файл на внешний GitHub репозиторий
git push

 7. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON
vim new.json
i
{
	"name":"John",
	"surname":"Smith",
	"age":27,
	"pets":{
					"number":1,
					"kind_of_pet":"cat",
					"name":"Klaus"
					},
	"desired_salary":"10000$"
}
esc
:wq

 8. Отправить изменения на внешний репозиторий
git add new.json ; git commit -m "update new.json" ; git push

 9. Создать файл preferences.json
touch preferences.json

 10. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON
vim preferences.json
i
{
	"movie":"Fight_club",
	"series":"Friends",
	"food":"borsch",
	"season":"spring",
	"country":"Portugal"
}
esc
:wq

 11. Создать файл sklls.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON
touch skills.json
vim skills.json
i
{
	"soft_skills":"patiens",
	"hard_skills":[
			"software testing theory",
			"client-server architecture",
			"scrum development methodology"
		      ]
}
esc
:wq

 12. Отправить сразу 2 файла на внешний репозиторий
git add . ; git commit -m "add 2 files: preferences.json, skills.json" ; git push

 13. На веб интерфейсе создать файл bug_report.json
Add file >> Create new file >> bug_report.json

 14. Сделать Commit changes (сохранить) изменения на веб интерфейсе
Commit new file

 15. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON
Edit this file
{
	"ID":1,
	"Project":"esculab.com",
	"Summary":"The text colour of the 'Get result' button merges with the background colour of the button when the cursor is hovered over the service page",
	"Actual result":"The text colour of the 'Get result' button merges with the background colour of the button when the cursor is hovered over the service page",
	"Expected result":"The colour of the 'Get result' button text becomes white when the cursor is hovered over the service page",
	"Pre-conditions":"Open the service page. Example https://...",
	"Steps to reproduce":"Place the cursor on the 'Get result' button",
	"Environment":"macOS BigSur v:11.2.3 Google Chrome v:94.0.4606.71 (x86_64)",
	"Severity":"Trivial",
	"Priority":"Low",
	"Status":"Submitted",
	"Attachments":"Video link",
	"Workaround":"No", 
	"Reproducibility":"Always"
}
 16. Сделать Commit changes (сохранить) изменения на веб интерфейсе
Commit changes

 17. Синхронизировать внешний и локальный репозиторий JSON
git pull
