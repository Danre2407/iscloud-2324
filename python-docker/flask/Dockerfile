FROM python:3.8-slim-buster

# Create app directory
WORKDIR /app

# Get the files
COPY app.py app.py
COPY requirements.txt requirements.txt

# Install dependencies
RUN pip3 install -r requirements.txt

# Export port
EXPOSE 5000
ENV MYSQL_ROOT_PASSWORD=test123

CMD [ "python3", "-m", "flask", "run", "--host=0.0.0.0" ]