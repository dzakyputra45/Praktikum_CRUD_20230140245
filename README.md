<p align="center">
  <img src="docs/api-preview.png" width="900"/>
</p>

<h1 align="center">📚 Documentation</h1>

<p align="center">
Dokumentasi endpoint REST API untuk project ini
</p>

---

# <img width="1919" height="968" alt="Screenshot 2026-03-04 121737" src="https://github.com/user-attachments/assets/d7212d82-33eb-4175-807f-69e910944558" />


http://localhost:8080

---

# 👤 User API

## 1️⃣ Add User

Menambahkan user baru.

**Endpoint**


POST [(http://localhost:8080/api/users)


**Request Body**

{
  "name": "Dzaky",
  "age": 21
}

Response

{
    "status": "success",
    "data": {
        "age": 24,
        "id": "e4ba5a2f-5f1b-4ce4-a025-716bbf6c5f6f",
        "name": "Dzaky Putra Pratama"
    }
}


2️⃣ Get All Users

Mengambil semua data user.

Endpoint

GET (http://localhost:8080/api/users)

Response

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


3️⃣ Get User By ID

Mengambil data user berdasarkan ID.

Endpoint

GET /users/{id}

Example

GET (http://localhost:8080/api/users/35ed3b55-663c-46d3-9453-bf20230fb07f)

Response

{
    "status": "success",
    "data": {
        "age": 21,
        "id": "35ed3b55-663c-46d3-9453-bf20230fb07f",
        "name": "Dzaky Putra Pratama"
    }
}


4️⃣ Update User

Mengupdate data user.

Endpoint

PUT (http://localhost:8080/api/users/35ed3b55-663c-46d3-9453-bf20230fb07f)

Request Body

{
  "name": "Dzaky Putra Pratama",
  "age": 23
}

Response

{
    "status": "success",
    "data": {
        "age": 23,
        "id": "35ed3b55-663c-46d3-9453-bf20230fb07f",
        "name": "Dzaky Putra Pratama"
    }
}


5️⃣ Delete User

Menghapus user berdasarkan ID.

Endpoint

DELETE (http://localhost:8080/api/users/35ed3b55-663c-46d3-9453-bf20230fb07f)

Response

{
    "status": "success delete user with id 35ed3b55-663c-46d3-9453-bf20230fb07f"
}
