FROM python:3.10-slim-buster

MAINTAINER Szkolenie LFD459

WORKDIR /app

COPY requirements.txt .

RUN pip3 install --no-cache-dir -r requirements.txt

RUN adduser flaskuser

COPY --chown=flaskuser:flaskuser . .

USER flaskuser

ENV PYTHONVAR="/path/to/sth"

CMD ["python3", "app.py"]
