FROM python:3.7.12-slim

RUN pip install --upgrade pip

COPY ./requirements.txt .
RUN pip install -r requirements.txt

WORKDIR /app
COPY . .

ENTRYPOINT ["sh", "/app/entrypoint.sh"]