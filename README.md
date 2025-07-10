# eco-13f-sec-filings-parser
Parse SEC Filings into HTML and XML Format

# Project Structure
sec13f/
├── app/
│   ├── api/               
│   ├── models/            
│   ├── services/           
│   ├── tasks/              
│   ├── db.py               
│   ├── main.py             
├── celery_worker.py        
├── requirements.txt
├── Dockerfile
└── README.md

# FastAPI route definitions. Server enpoints for filings and holdings
# SQLAlchemy models. Define model and interact with PostgreSQL
# XML parsing, SEC fetching logic. lxml or xml.etree to parse 13f XML filings
# Celery background jobs - Celery Beat or APScheduler to auotmate daily/weekly fetches
# DB connection/session - SQLAlchemy
# FastAPI app entry point
# Celery worker runner
