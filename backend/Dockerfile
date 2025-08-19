FROM python:3.11

WORKDIR /app

COPY requirements.txt .

RUN pip install gunicorn==23.0.0 

RUN pip install -r requirements.txt --no-cache-dir

COPY . .

CMD ["python", "manage.py", "runserver", "0:8000"]