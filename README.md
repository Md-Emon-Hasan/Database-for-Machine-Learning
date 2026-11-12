# Database for Machine Learning

[![Python](https://img.shields.io/badge/Python-3.9%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/API-FastAPI-009688?logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-4169E1?logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![MongoDB](https://img.shields.io/badge/Database-MongoDB-47A248?logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![MySQL](https://img.shields.io/badge/Database-MySQL-4479A1?logo=mysql&logoColor=white)](https://www.mysql.com/)
[![MariaDB](https://img.shields.io/badge/Database-MariaDB-003545?logo=mariadb&logoColor=white)](https://mariadb.org/)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)

A hands-on repository where I document my learning about Python databases. I have brought together relational database examples, MongoDB notebooks, and a FastAPI + PostgreSQL CRUD starter to practice these concepts in code.

## Repository modules

| Module | What it contains | Main technologies |
| --- | --- | --- |
| [FastAPI with PostgreSQL](Fastapi-with-PostgreSQL/) | A small user API with create/list endpoints, SQLAlchemy models, Pydantic schemas, and PostgreSQL configuration. | FastAPI, PostgreSQL, SQLAlchemy, Uvicorn |
| [Python with MongoDB](Python-with-MongoDB/) | Jupyter notebooks for connecting, querying, updating, and aggregating MongoDB documents. | Python, PyMongo, Jupyter |
| [Python with MySQL & MariaDB](Python-with-MySQL-MariaDB/) | Numbered Python exercises for database setup, CRUD, filtering, joins, and aggregate queries. | Python, PyMySQL, MySQL, MariaDB |

## Getting started

Each module is independent and has its own instructions. Clone this repository, then follow the relevant module guide:

```bash
git clone https://github.com/Md-Emon-Hasan/Database-for-Machine-Learning.git
cd Database-for-Machine-Learning
```

### FastAPI + PostgreSQL

1. Install and start PostgreSQL, then create a development database (the example configuration uses `fastapi_db`).
2. Create and activate a virtual environment, then install the API dependencies:

   ```bash
   cd Fastapi-with-PostgreSQL
   python -m venv .venv
   # Windows PowerShell: .\.venv\Scripts\Activate.ps1
   # macOS/Linux: source .venv/bin/activate
   python -m pip install -r requirements.txt
   ```

3. Copy `.env.example` to `.env` and set `DATABASE_URL` to match your local PostgreSQL credentials. Keep `.env` private.
4. Start the development server:

   ```bash
   uvicorn app.main:app --reload
   ```

   Open `http://127.0.0.1:8000/docs` for the interactive API documentation. See [the module README](Fastapi-with-PostgreSQL/readme.md) for endpoints and configuration details.

### MongoDB notebooks

Install a MongoDB server or prepare an Atlas database, then install Python, PyMongo, and Jupyter:

```bash
python -m pip install pymongo notebook
```

Launch Jupyter from `Python-with-MongoDB/`, configure the connection URI in the notebook, and run the notebook cells in order. Start with the [MongoDB module guide](Python-with-MongoDB/README.md).

### MySQL / MariaDB exercises

Install and start MySQL or MariaDB, then install PyMySQL:

```bash
python -m pip install PyMySQL
```

Update the local connection settings in the scripts and follow the numbered examples in [the MySQL/MariaDB guide](Python-with-MySQL-MariaDB/README.md). Some later join and aggregate examples expect tables that are not created by the introductory scripts.

## What I have included in this repository

- **A FastAPI + PostgreSQL starter API** that creates and lists users, with the code split into routes, CRUD operations, models, schemas, and database configuration.
- **MongoDB notebooks** that walk through connecting from Python, querying JSON documents, updating records, and aggregating data.
- **MySQL/MariaDB scripts** that demonstrate database setup, CRUD operations, filtering, joins, and common SQL aggregate functions.

## What I'm learning

- How I can connect Python applications to PostgreSQL, MongoDB, MySQL, and MariaDB
- How relational tables and MongoDB documents differ, and how to query each
- How to create, read, update, and delete data in practice
- How to write SQL filters, joins, and aggregate queries
- How a FastAPI endpoint validates input and uses SQLAlchemy with PostgreSQL

## How this repository supports my learning

I use this repository to learn database concepts through hands-on examples, starting with basic connections and moving on to queries and a small API. I can study each module independently, follow the numbered SQL scripts and ordered notebooks step by step, and see how database operations fit into a backend application. I can also adapt these examples as I build my own learning projects.

## Project layout

```text
Database-for-Machine-Learning/
├── Fastapi-with-PostgreSQL/   # FastAPI user CRUD API
├── Python-with-MongoDB/       # MongoDB learning notebooks
├── Python-with-MySQL-MariaDB/ # SQL and Python exercises
├── LICENSE
└── README.md
```

## Contributing

Issues, corrections, and additional database examples are welcome. Please open an issue to discuss a larger change, or submit a pull request with a clear description of what you changed.

## License

This repository is distributed under the [Apache License 2.0](LICENSE).

## Connect with me

- 🌐 **Portfolio:** [emonlabs-ai.hitechparks.com](https://emonlabs-ai.hitechparks.com)
- 💻 **GitHub:** [Md-Emon-Hasan](https://github.com/Md-Emon-Hasan)
- 💼 **LinkedIn:** [Md Emon Hasan](https://www.linkedin.com/in/md-emon-hasan-695483237/)
- 🤗 **Hugging Face:** [emonHasan01](https://huggingface.co/emonHasan01)
- 📧 **Email:** [emon.mlengineer@gmail.com](mailto:emon.mlengineer@gmail.com)
- 📱 **WhatsApp:** [+8801834363533](https://wa.me/8801834363533)
