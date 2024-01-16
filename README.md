**Требования к запуску API коллекции: ОС Windows(x86), Postman актуальной версии.**
>Установите Postman на свою локальную машину. 
Скачайте файл в формате .json из данного репозитория и импортируйте этот файл в Postman.
Коллекция по API Postman в данном файле представлена по следующему сценарию:

- Создать issue с названием Issue 1 (Post)
- Получить список issues (Get)
- Изменить название задачи на Issue 2 (Patch)
- Удалить Issue 2 (Delete)

# GitHub 
 
Описание проекта : Сайт GitHub (https://github.com/) 
 
Это Postman коллекция предназначена для тестирования API GitHub issues  
 
 
## Использование 
1. Установите Postman (https://www.postman.com/downloads/) на свой компьютер 
2. Скачайте текущую коллекцию. 
3. Импортируйте коллекцию в Postman. 
4. В Autorization добавьте Bearer Token - ваш токен GitHub. 
 
 
## Переменные среды 
- token - ваш токен GitHub. 
- Repo  - название вашего репозитория. 
- Owner - ваш ник на GitHub. 
- GitHub - api GitHub: https://api.github.com/ 
 
 
 
## Описание запросов 
   1. Создание issue: 
   - Описание: Создает новую задачу в репозитории GitHub. 
   - Путь: /repos/{owner}/{repo}/issues 
   - Метод: POST 
   2. Получение списка задач: 
   - Описание: Возвращает список задач из репозитория GitHub. 
   - Путь: /repos/{owner}/{repo}/issues 
   - Метод: GET 
   3. Изменение названия задачи: 
   - Описание: Изменяет название существующей задачи в репозитории GitHub. 
   - Путь: /repos/{owner}/{repo}/issues/{issue_number} 
   - Метод: PATCH 
  4. Удаление задачи: 
   - Описание: Удаляет существующую задачу из репозитория GitHub. 
   - Путь: /repos/{owner}/{repo}/issues/{issue_number}/lock 
   - Метод: DELETE 
 
В Запросах 'POST'  'PATCH' используется  
Body { 
  "title": "Issue", 
  "body": "Something went wrong.", 
  "labels": ["bug"], 
  "assignees": ["Ваш ник на GIT"] 
} 
## 
Ссылка на Git 
https://github.com/Gipsoday/test.git
