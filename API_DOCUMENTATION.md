# 📡 API Documentation — Campus Backend

---

## 🌐 Base URL

```
http://localhost:8080
```

---

## 👨‍🎓 Student APIs

### 🔹 Submit Complaint

POST `/student/complaint`

```json
{
  "email": "student@email.com",
  "title": "Water leakage",
  "description": "Pipe leaking in hostel",
  "imageUrl": "image_link",
  "priority": "HIGH"
}
```

---

### 🔹 Get My Complaints

GET `/student/complaints?email=student@email.com`

---

## 🏢 Department APIs

### 🔹 Login

POST `/dept/login`

```json
{
  "email": "it@sitpune.edu.in",
  "password": "dept@123"
}
```

---

### 🔹 Get Department Complaints

GET `/dept/complaints/{departmentId}`

---

### 🔹 Resolve Complaint

POST `/dept/resolve`

```json
{
  "complaintId": 1,
  "resolvedImageUrl": "image_link"
}
```

---

## 🧑‍💼 Admin APIs

### 🔹 Get All Complaints

GET `/admin/complaints?page=0&size=10`

---

### 🔹 Update Status

PUT `/admin/status`

```json
{
  "complaintId": 1,
  "status": "IN_PROGRESS"
}
```

---

### 🔹 Dashboard Stats

GET `/admin/stats`

---

## 🔄 Complaint Flow

```
PENDING → ASSIGNED → IN_PROGRESS → RESOLVED → CLOSED
```

---

## ⚠️ Notes

* JWT authentication not implemented yet
* APIs are open for testing
