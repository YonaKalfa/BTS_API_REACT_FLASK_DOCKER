from python:3.11-alpine

run apk add --no-cache gcc musl-dev libpq

workdir /app

copy requirements.txt /app/requirements.txt
run pip install --no-cache-dir -r /app/requirements.txt

expose 5000

cmd ["sh", "-c", "flask run --host=0.0.0.0 --port=5000"]