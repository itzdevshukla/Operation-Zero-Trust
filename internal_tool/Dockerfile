FROM python:3.9-slim
WORKDIR /app
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
# Running as root to allow flag reading, but in a real scenario, this would just be the app user.
EXPOSE 5000
CMD ["python", "app.py"]
