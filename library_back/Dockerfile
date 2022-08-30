FROM python:latest

ENV PYTHONUNBUFFERED 1

RUN mkdir /library_db

WORKDIR /library_db

COPY requirements.txt .

RUN pip install -r requirements.txt

COPY . .

ENTRYPOINT ["tail","-f","/dev/null"]