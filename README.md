# 🏫 Campus Complaint Management Backend

A Spring Boot backend system where students can report campus issues with images, and complaints are automatically routed to the correct department for resolution.

---

## 🚀 Features

* 👨‍🎓 Student complaint submission (with image)
* 🏢 Auto department assignment (AI keyword-based)
* 🛠 Department resolves complaints
* 🧑‍💼 Admin monitors all complaints
* 🔐 BCrypt password security
* 📊 Dashboard stats
* 📄 Pagination support
* 📧 Email notification on resolution
* ✅ 25+ unit tests

---

## 🛠 Tech Stack

* Java 17
* Spring Boot
* Spring Data JPA
* PostgreSQL (Supabase)
* Maven
* JUnit + Mockito

---

## 📁 Project Structure

```
campusbackend/
 ├── src/
 ├── pom.xml
 ├── .gitignore
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone Repo

```
git clone https://github.com/rafin-110/campus_backend.git
cd campus_backend/campusbackend
```

---

### 2️⃣ Configure Environment Variables

Create `.env` or update `application.properties`:

```
DB_URL=your_supabase_url
DB_USERNAME=postgres
DB_PASSWORD=your_password
MAIL_USERNAME=your_email
MAIL_APP_PASSWORD=your_app_password
JWT_SECRET=your_secret
```

---

### 3️⃣ Run Project

```
mvn clean install
mvn spring-boot:run
```

---

### 4️⃣ Seed Database

Run `seed_departments.sql` in Supabase SQL editor.

---

## 🌐 Base URL

```
http://localhost:8080
```

---

## 🧪 Testing

```
mvn test
```

---

## 📌 Future Improvements

* JWT Authentication
* Role-based security
* File upload to cloud storage
* Frontend integration

---

## 👨‍💻 Author

* Rafin
