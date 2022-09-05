FROM python:latest

WORKDIR /library_db

COPY ./requirements.txt .

RUN pip install -r requirements.txt

COPY . .

EXPOSE 8000