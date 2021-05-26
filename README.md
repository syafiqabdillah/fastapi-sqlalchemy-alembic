# FastAPI + SQL Alchemy practice
## Installation
1. clone this repo
2. create virtual environtment

```bash
# for windows

$ python -m virtualenv venv

$ venv\Script\activate

# for linux / macOS

$ python3 -m virtualenv venv

source venv/bin/activate
```
3. install all dependencies 
```bash
(venv) $ pip install -r requirements.txt
```
4. add `.env` file, look at `.env.example` file
5. run migration with alembic

```bash
(venv) $ alembic revision -m "First migration"

(venv) $ alembic upgrade head
```
6. run the server 
```bash
(venv) $ uvicorn main:app --reload
```
