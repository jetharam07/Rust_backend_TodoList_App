# Rust_backend_TodoList_App

# 📝 Todo App in Rust using Rocket

This is a simple RESTful Todo application developed using the [Rocket](https://rocket.rs/) web framework in Rust. It allows you to perform basic CRUD operations (Create, Read, Update, Delete) on tasks, which are saved in a CSV file. This is a minimal example of building an HTTP API with Rocket and Serde.

---

## 🚀 Key Features

- Task persistence using a `tasks.csv` file
- REST API to create, view, update, and delete todos
- Live-reload enabled during development using `cargo watch`
- JSON support via Rocket and Serde integration

---

## 🧱 Built With

This project makes use of the following Rust libraries (crates):

- **[rocket](https://crates.io/crates/rocket)** – v0.5.1 (includes JSON support)
- **[serde](https://crates.io/crates/serde)** – v1.0.219 (with `derive` feature)
- **[csv](https://crates.io/crates/csv)** – v1.3.1

## 📁 Project Structure

```
.
├── src/
├── .gitignore
├── Cargo.lock
├── Cargo.toml
├── README.md
└── tasks.csv
```

---

## 🛠️ Getting Started

To run the app with live-reloading, make sure you have `cargo-watch` installed:

```bash
cargo install cargo-watch
```

Then run the project with:

```bash
cargo watch -x run
```

---

## 📘 API Endpoints

| Method | Endpoint     | Description         |
|--------|--------------|---------------------|
| GET    | /tasks       | Get all tasks  |
| POST   | /tasks       | Add a new task      |
| PUT    | /tasks/&lt;id&gt; | Update task     |
| DELETE | /tasks/&lt;id&gt; | Delete task     |
