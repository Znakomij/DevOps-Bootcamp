FROM python:3.9-slim

ENV CONTAINERENV True
EXPOSE 5000

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

COPY app.py app.py
COPY /templates/index.html /templates/index.html
COPY mail.txt mail.txt
COPY name.txt name.txt

ENTRYPOINT python3 app.py
