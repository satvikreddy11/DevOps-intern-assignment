
FROM python:3.13-slim


WORKDIR /app


COPY . .


RUN pip install --upgrade pip && pip install .


EXPOSE 8002


CMD ["python", "app.py"]