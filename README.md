Задание 1
1)Были использованы следующие для ввода данные: логин:' or 1=1;--  пароль: любой 
2)удолось войти под админом
3)SQL-инъекция обходит проверку пароля, делая условие всегда истинным
4) Где хранится:
Cookies (Куки) - основной способ хранения
LocalStorage - дополнительные данные
SessionStorage - временные данные сессии

Что представляет из себя:
В Cookies:
Ключ: token
Значение: JWT-токен в формате Base64, содержащий:

В LocalStorage:
token - дублирование JWT-токена
email - email пользователя
bid - ID корзины (basket ID)

Как передаётся в каждом запросе:
Механизм передачи:
Автоматически браузером в заголовке Cookie: token=your_jwt_token
В REST API запросах - в заголовке Authorization: Bearer your_jwt_token

СКРИНЫ:<img width="1918" height="1001" alt="image" src="https://github.com/user-attachments/assets/e653e354-05a2-4b5d-916e-e3d15e76f62e" />
        <img width="1920" height="999" alt="image" src="https://github.com/user-attachments/assets/a6817289-9697-4953-8de7-6233021ef408" />

