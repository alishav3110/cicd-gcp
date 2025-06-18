FROM python:3.8
EXPOSE 8080
WORKDIR /app

# Copy just requirements first for better caching
COPY app/requirements.txt ./
RUN pip install -r requirements.txt

# Then copy the rest of the app files
COPY app/ ./

CMD ["python", "app.py"]
