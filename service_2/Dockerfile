FROM python:3.9-slim

WORKDIR /app

COPY . .

# ✅ Install Flask and curl directly
RUN pip install flask && apt-get update && apt-get install -y curl

EXPOSE 8002

CMD ["python", "app.py"]