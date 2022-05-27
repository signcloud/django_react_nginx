FROM python:3.9
ENV PYTHONUNBUFFERED=1
WORKDIR /backend

RUN pip install pipenv
COPY . .
RUN pip install -r requirements.txt
COPY server/entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh

COPY server /backend/