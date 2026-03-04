<h1 align="center">📚 Documentation</h1>

<p align="center">
Dokumentasi endpoint REST API untuk project ini
</p>

---

# <img width="1919" height="968" alt="Screenshot 2026-03-04 121737" src="https://github.com/user-attachments/assets/d7212d82-33eb-4175-807f-69e910944558" />

---

## 🌐 Base URL

`http://localhost:8080/api`

---

## 📌 Endpoint Summary

| Method | Endpoint    | Description    |
| ------ | ----------- | -------------- |
| POST   | /users      | Add new user   |
| GET    | /users      | Get all users  |
| GET    | /users/{id} | Get user by ID |
| PUT    | /users/{id} | Update user    |
| DELETE | /users/{id} | Delete user    |

---

# 👤 User API

---

## 1️⃣ Add User

Menambahkan user baru.

**Endpoint**

POST /users

**Full URL**

http://localhost:8080/api/users

**Request Body**

```json
{
  "name": "Dzaky",
  "age": 21
}
```

**Response**

```json
{
  "status": "success",
  "data": {
    "age": 21,
    "id": "e4ba5a2f-5f1b-4ce4-a025-716bbf6c5f6f",
    "name": "Dzaky Putra Pratama"
  }
}
```

---

## 2️⃣ Get All Users

Mengambil semua data user.

**Endpoint**

GET /users

**Full URL**

http://localhost:8080/api/users

**Response**

```json
{
  "status": "success",
  "data": [
    {
      "age": 21,
      "id": "35ed3b55-663c-46d3-9453-bf20230fb07f",
      "name": "Dzaky Putra Pratama"
    },
    {
      "age": 21,
      "id": "4715e83b-c26c-46b8-b8da-1e7b948e3067",
      "name": "JACK"
    },
    {
      "age": 24,
      "id": "e4ba5a2f-5f1b-4ce4-a025-716bbf6c5f6f",
      "name": "Dzaky Putra Pratama"
    }
  ]
}
```

---

## 3️⃣ Get User By ID

Mengambil data user berdasarkan ID.

**Endpoint**

GET /users/{id}

**Example URL**

http://localhost:8080/api/users/35ed3b55-663c-46d3-9453-bf20230fb07f

**Response**

```json
{
  "status": "success",
  "data": {
    "age": 21,
    "id": "35ed3b55-663c-46d3-9453-bf20230fb07f",
    "name": "Dzaky Putra Pratama"
  }
}
```

---

## 4️⃣ Update User

Mengupdate data user.

**Endpoint**

PUT /users/{id}

**Example URL**

http://localhost:8080/api/users/35ed3b55-663c-46d3-9453-bf20230fb07f

**Request Body**

```json
{
  "name": "Dzaky Putra Pratama",
  "age": 23
}
```

**Response**

```json
{
  "status": "success",
  "data": {
    "age": 23,
    "id": "35ed3b55-663c-46d3-9453-bf20230fb07f",
    "name": "Dzaky Putra Pratama"
  }
}
```

---

## 5️⃣ Delete User

Menghapus user berdasarkan ID.

**Endpoint**

DELETE /users/{id}

**Example URL**

http://localhost:8080/api/users/35ed3b55-663c-46d3-9453-bf20230fb07f

**Response**

```json
{
  "status": "success",
  "message": "User deleted successfully"
}
```

---

Dzaky Putra
