FROM python:3.10

WORKDIR /app

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY . .

RUN mkdir -p /app/data

CMD ["gunicorn", "--bind", "0.0.0.0:8000", "backend.wsgi:application"]