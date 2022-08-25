FROM python:latest

ENV PYTHONUNBUFFERED 1

WORKDIR /backend

COPY requirements.txt .

RUN pip install -r requirements.txt

COPY . .

CMD ["python", "manage.py", "makemigrations", "&&", "python", "manage.py", "migrate", "&&", "python", "manage.py", "runserver"]

ENTRYPOINT ["tail","-f","/dev/null"]