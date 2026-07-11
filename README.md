# Rewire — ThoughtWorks Internship Project

Full-stack CBT (Cognitive Behavioral Therapy) thought journal with social justice "Know Your Rights" educational content. Built during the 2022 ThoughtWorks social-justice internship by a team of ~12.

---

## What it does

Users submit four-part CBT thoughts through a React frontend. The Spring Boot backend stores them in PostgreSQL. The app also includes FAQ, tutorials, and rights information for marginalized communities.

---

## Tech stack

**Backend:**
- Java 11, Spring Boot 2.4.4
- Spring Data JPA, PostgreSQL, HikariCP
- Lombok

**Frontend (`internship-project/app/`):**
- React 17, Material-UI v4 + MUI v5
- Axios

---

## Quick start

### Prerequisites

- Java 11, Node.js/npm, PostgreSQL

### Backend

```bash
git clone https://github.com/Kaireega/ThoughtWorks-internship-mainProjects-.git
cd ThoughtWorks-internship-mainProjects-/internship-project

# Set database credentials via environment variables:
export username=your_db_user
export password=your_db_password

./mvnw spring-boot:run
```

### Frontend

```bash
cd internship-project/app
npm install
npm start    # Proxies API to localhost:8080
```

### API

| Endpoint | Method | Body |
|----------|--------|------|
| `GET /api/cbt` | GET | — (list all thoughts) |
| `POST /api/cbt` | POST | `{ "firstThought", "secondThought", "thirdThought", "fourthThought" }` |

---

## Project structure

```
ThoughtWorks-internship-mainProjects-/
└── internship-project/
    ├── pom.xml
    ├── src/main/java/com/example/demo/    # Spring Boot backend
    ├── app/                                # React frontend (npm: "rewire")
    ├── docs/                               # Content and check-in notes
    └── LICENSE.txt
```

For detailed ThoughtWorks onboarding docs, see [`internship-project/readme.md`](internship-project/readme.md).

---

## Author

**Kai'ree Gay** — [GitHub](https://github.com/Kaireega)
