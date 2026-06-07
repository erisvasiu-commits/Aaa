eveng-backend/
├── main.py                    # Entry point
├── requirements.txt           # Varësitë
├── seed.py                    # Popullo databazën me të dhëna demo
├── eveng.db                   # SQLite databaza (krijohet automatikisht)
└── app/
    ├── database.py            # Lidhja me SQLite
    ├── models.py              # Tabelat (User, Project, Task, Plan, TeamMember)
    ├── schemas.py             # Pydantic schemas (validim + serialiizm)
    ├── auth.py                # JWT tokens + kontroll rolesh
    └── routers/
        ├── auth_router.py     # POST /auth/login, /auth/register, GET /auth/me
        ├── users.py           # CRUD /users (admin)
        ├── projects.py        # CRUD /projects
        ├── tasks.py           # CRUD /tasks
        └── plans_team.py      # CRUD /plans dhe /team
