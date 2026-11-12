# FastAPI with PostgreSQL

[![Python](https://img.shields.io/badge/Python-3.9%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/API-FastAPI-009688?logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-4169E1?logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![SQLAlchemy](https://img.shields.io/badge/ORM-SQLAlchemy-D71F00?logo=sqlalchemy&logoColor=white)](https://www.sqlalchemy.org/)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](../LICENSE)

A small synchronous FastAPI + PostgreSQL example for learning API and database fundamentals. It demonstrates a modular app structure, SQLAlchemy ORM models, Pydantic request/response schemas, and basic user creation and listing endpoints.

## Features

- FastAPI application with interactive OpenAPI documentation
- PostgreSQL connection configured through `DATABASE_URL`
- SQLAlchemy model for users (`id`, `name`, `email`)
- Create and list user endpoints under `/users`
- Pydantic schemas for request validation and response serialization

## Requirements

- Python 3.9 or newer
- PostgreSQL server and a database (default name: `fastapi_db`)

## Setup

1. From the repository root, enter this module and create a virtual environment:

   ```bash
   cd Fastapi-with-PostgreSQL
   python -m venv .venv
   # Windows PowerShell: .\.venv\Scripts\Activate.ps1
   # macOS/Linux: source .venv/bin/activate
   ```

2. Install dependencies:

   ```bash
   python -m pip install -r requirements.txt
   ```

3. Create a PostgreSQL database:

   ```sql
   CREATE DATABASE fastapi_db;
   ```

4. Copy `.env.example` to `.env`, then set `DATABASE_URL` to match your PostgreSQL username, password, host, and database. For example:

   ```env
   DATABASE_URL=postgresql://postgres:your_password@localhost:5432/fastapi_db
   ```

   Keep `.env` out of version control. URL-encode special characters in the password when needed.

## Run the API

Start the development server from this module directory:

```bash
uvicorn app.main:app --reload
```

The API runs at `http://127.0.0.1:8000`. Interactive documentation is available at `/docs` and `/redoc`.

## Endpoints

| Method | Path | Description | Example request body |
| --- | --- | --- | --- |
| `GET` | `/` | Health/status response | — |
| `POST` | `/users/` | Create a user | `{"name": "Ada Lovelace", "email": "ada@example.com"}` |
| `GET` | `/users/` | List users | — |

The app creates tables from the SQLAlchemy models when it starts. This is a learning example; it does not currently include schema migrations, authentication, or production deployment configuration.

## Project structure

```text
app/
├── main.py       # FastAPI app and router registration
├── database.py   # PostgreSQL engine and session dependency
├── models.py     # SQLAlchemy models
├── schemas.py    # Pydantic schemas
├── crud.py       # Database operations
└── routers/
    └── user.py   # User API routes
```

## License

Distributed under the [Apache License 2.0](../LICENSE).

## Connect with me

- 🌐 **Portfolio:** [emonlabs-ai.hitechparks.com](https://emonlabs-ai.hitechparks.com)
- 💻 **GitHub:** [Md-Emon-Hasan](https://github.com/Md-Emon-Hasan)
- 💼 **LinkedIn:** [Md Emon Hasan](https://www.linkedin.com/in/md-emon-hasan-695483237/)
- 🤗 **Hugging Face:** [emonHasan01](https://huggingface.co/emonHasan01)
- 📧 **Email:** [emon.mlengineer@gmail.com](mailto:emon.mlengineer@gmail.com)
- 📱 **WhatsApp:** [+8801834363533](https://wa.me/8801834363533)
