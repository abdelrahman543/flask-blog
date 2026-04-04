# 📝 Flask Blog Platform

A full-stack blogging web application built with Flask. Supports user authentication, rich-text post creation, commenting, and admin-only controls — all backed by a SQLite database.

---

## ✨ Features

- 🔐 **User Authentication** — register, login, and logout with hashed passwords
- 🛡️ **Admin Panel** — only the first registered user can create, edit, or delete posts
- ✍️ **Rich Text Editor** — write posts with full formatting using CKEditor
- 💬 **Comments** — authenticated users can comment on any post
- 🖼️ **Gravatar Integration** — user avatars auto-generated from email
- 🗄️ **SQLite Database** — relational data with Users, Posts, and Comments tables
- ⚡ **Flask-Bootstrap 5** — clean, responsive UI out of the box

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3 | Core language |
| Flask | Web framework |
| Flask-SQLAlchemy | ORM & database management |
| Flask-Login | User session management |
| Flask-CKEditor | Rich text editor |
| Flask-Bootstrap 5 | Responsive UI components |
| Werkzeug | Password hashing |
| SQLite | Local database |

---

## 🚀 Getting Started

### 1. Install dependencies
```bash
pip install -r requirements.txt
```

### 2. Run the app
```bash
python main.py
```

### 3. Open in browser
```
http://localhost:5001
```

> The first account you register automatically becomes the **admin**.

---

## 📁 Project Structure

```
flask-blog/
├── main.py              # App entry point, routes & models
├── forms.py             # WTForms form classes
├── requirements.txt     # Python dependencies
├── instance/
│   └── posts.db         # SQLite database (auto-created)
└── templates/
    ├── index.html
    ├── post.html
    ├── register.html
    ├── login.html
    ├── make-post.html
    ├── about.html
    └── contact.html
```

---

## 📸 Preview

*(Add a screenshot here — save it as `preview.png` in the repo root)*

![Blog Preview](preview.png)

---

## 🔒 Security Note

Before deploying to production:
- Move `SECRET_KEY` to an environment variable — never hardcode it
- Switch from SQLite to PostgreSQL for production use
- Set `debug=False` in `app.run()`

---

## 📌 Roadmap

- [ ] Move secret key to `.env` file
- [ ] Add pagination for posts
- [ ] Add post categories / tags
- [ ] Deploy to Railway or Render
- [ ] Add email contact form functionality

---

## 👨‍💻 Author

**Abdelrahman**
