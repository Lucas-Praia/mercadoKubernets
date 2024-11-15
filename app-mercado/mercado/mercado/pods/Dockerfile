
FROM python:3.10.15-slim


WORKDIR /app


RUN apt-get update && apt-get install -y \
    build-essential \
    python3-dev \
    && apt-get clean \
    && apt-get autoremove -y \
    && rm -rf /var/lib/apt/lists/*


COPY requirements.txt .


RUN pip install --upgrade pip && \
    pip install --no-cache-dir -r requirements.txt


COPY . .


EXPOSE 8000


CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]