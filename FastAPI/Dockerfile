FROM python:3.9-alpine3.21
WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .
EXPOSE 3000
CMD [ "fastapi", "dev", "main.py" ]