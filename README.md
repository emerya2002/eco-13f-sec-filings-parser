# eco-13f-sec-filings-parser
Parse SEC Filings into HTML and XML Format

# Project Structure
sec13f/
├── app/
│   ├── api/                # FastAPI route definitions. Server enpoints for filings and holdings
│   ├── models/             # SQLAlchemy models. Define model and interact with PostgreSQL
│   ├── services/           # XML parsing, SEC fetching logic. lxml or xml.etree to parse 13f XML filings
│   ├── tasks/              # Celery background jobs - Celery Beat or APScheduler to auotmate daily/weekly fetches
│   ├── db.py               # DB connection/session - SQLAlchemy
│   ├── main.py             # FastAPI app entry point
├── celery_worker.py        # Celery worker runner
├── requirements.txt
├── Dockerfile
└── README.md
