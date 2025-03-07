## Методы API

### 1. Создание пользователя
- **URL:** `/api/users/`
- **Метод:** `POST`
- **Тело запроса:**
  ```json
  {
    "username": "string",
    "password": "string",
    "email": "string"
  }
  ```
- **Ответ:**
  ```json
  {
    "status": "User created!"
  }
  ```

### 2. Обновление информации о пользователе
- **URL:** `/api/users/{id}`
- **Метод:** `PUT`
- **Тело запроса:**
  ```json
  {
    "username": "string",
    "password": "string",
    "email": "string"
  }
  ```
- **Ответ:**
  ```json
  {
    "status": "User updated!"
  }
  ```

### 3. Удаление пользователя
- **URL:** `/api/users/{id}`
- **Метод:** `DELETE`
- **Ответ:**
  ```json
  {
    "status": "User deleted"
  }
  ```

### 4. Получение информации о пользователе
- **URL:** `/api/users/{id}`
- **Метод:** `GET`
- **Ответ:**
  ```json
  {
    "id": "integer",
    "username": "string",
    "email": "string",
    "createdAt": "datetime",
    "updatedAt": "datetime"
  }
  ```

### 5. Авторизация пользователя
- **URL:** `/api/users/login`
- **Метод:** `POST`
- **Тело запроса:**
  ```json
  {
    "username": "string",
    "password": "string"
  }
  ```
- **Ответ:**
  ```json
  {
    "status": "Login successful"
  }
  ```
