FROM python:3.8
EXPOSE 8080
WORKDIR /app

# Copy requirements first (relative to Dockerfile location)
COPY app/requirements.txt .
RUN pip install -r requirements.txt

# Copy all app files (relative to Dockerfile location)
COPY app.py .
COPY . .

CMD ["python", "app.py"]
