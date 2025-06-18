FROM python:3.8
EXPOSE 8080
WORKDIR /app

# First copy just requirements.txt
COPY ../requirements.txt ./  # Note the relative path
RUN pip install -r requirements.txt

# Then copy the rest of the app
COPY . ./

CMD ["python", "app.py"]
