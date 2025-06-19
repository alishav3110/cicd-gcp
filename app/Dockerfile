# FROM python:3.8
# EXPOSE 8080
# WORKDIR /app

# # Copy requirements first (relative to Dockerfile location)
# COPY app/requirements.txt .
# RUN pip install -r requirements.txt

# # Copy all app files (relative to Dockerfile location)
# COPY app/app.py .
# COPY . .

# CMD ["python", "app.py"]
FROM python:3.8-slim
EXPOSE 8080
WORKDIR /app
COPY app/requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY app/app.py .
COPY app/templates/ ./templates/
CMD ["python", "app.py"]
