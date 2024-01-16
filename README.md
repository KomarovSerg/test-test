# GitHub 
 
Описание проекта : Сайт GitHub (https://github.com/) 
 
Эта Postman-коллекция предназначена для тестирования API GitHub issues  
 
 
## Использование 
1. Установить Postman (https://www.postman.com/downloads/) на свой компьютер 
2. Скачать текущую коллекцию. 
3. Импортировать коллекцию в Postman. 
4. В Autorization добавить Bearer Token - ваш токен GitHub. 
 
 
## Переменные среды 
- myToken - ваш токен GitHub. 
- repo  - название вашего репозитория. 
- owner - ваш логин на GitHub. 
- baseUrl - API GitHub: https://api.github.com/ 
 
  
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
   - Путь: /repos/{owner}/{repo}/issues/{issue_number} 
   - Метод: DELETE 
 
В Запросах 'POST' и 'PATCH' используется Body:
```
{ 
  "title": "Issue", 
  "body": "Something went wrong.", 
  "labels": ["bug"], 
  "assignees": ["Ваш логин на GitHub"] 
}
```
## 
Ссылка на Git 
https://github.com/KomarovSerg/test-test.git
