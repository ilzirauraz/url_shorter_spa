FROM python:3.8

ENV PYTHONUNBUFFERED 1

WORKDIR /app
COPY . .

RUN pip install --upgrade pip && pip install -r requirements.txt
CMD python manage.py migrate && python manage.py runserver 0.0.0.0:8000
