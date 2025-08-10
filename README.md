# Mock Server

A Spring Boot–based **Mock Server** for simulating API endpoints and responses — useful for rapid prototyping, integration testing, and frontend development without depending on live backend services.

---

## 📌 Features
- 🚀 Create and manage mock API endpoints easily
- 📦 Persistent storage with **MongoDB / DocumentDb**
- ⚡ Fast caching & session handling with **Redis/ECS**
- 🛠 Fully configurable responses (status, headers, body)
- ✅ Enforced code style with **Spotless** (Google Java Format)
- 🔄 Docker support for local development

---

## 🖥 Local Development Setup

### 1️⃣ Prerequisites
Make sure you have the following installed locally:
- **Java 21+** → `java -version`
- **Gradle** (or use the included `./gradlew` wrapper)
- **Docker** → for running MongoDB & Redis locally
- **Git** → to clone the repository

---

### 2️⃣ Clone the Repository
git clone https://github.com/umang0704/mock-server.git
cd mock-server
---

### 3. Configure Environment Variables

---

### 4. Start Dependencies

---

### 5. Build & Run the Application

Using Gradle wrapper:

```./gradlew build```

```./gradlew bootRun```

---

### 6. Run Tests

```./gradlew test```

---

### 7. Formatting and Code Style (Spotless)

We use [Spotless](https://github.com/diffplug/spotless) to enforce code formatting.  
**The build will fail if formatting is not applied.**

Check formatting:

```./gradlew spotlessCheck```

Auto-format code:

```./gradlew spotlessApply```

---

### 8. Stop Services

If you started dependencies via Docker:

```docker compose down```

---

## 🤝 Contributing

Contributions are welcome!
1. Fork the repo
2. Create a feature branch
3. Ensure code is formatted: `./gradlew spotlessApply`
4. Commit your changes
5. Open a pull request with a clear description
---

## 📅 Changelog

All notable changes are documented in [`CHANGELOG.md`](CHANGELOG.md), following the [Keep a Changelog](https://keepachangelog.com/) format.

---

## 🙌 Tips

Run this before committing to ensure everything is good:
`./gradlew clean check`