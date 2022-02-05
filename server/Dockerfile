# Set base image (host OS)
FROM python:3.9

# By default, listen on port 5000
EXPOSE 5000/tcp

# Copy the dependencies file to the working directory
COPY requirements.txt .

# Install any dependencies
RUN pip install -r requirements.txt
RUN pip install gunicorn

# Copy src folder to app folder
COPY src/ /app

#Set working dic to /app
WORKDIR /app

# Specify the command to run on container start
#CMD [ "python", "./app.py" ]

# 4 - Set env to port 8080 - Cloudrun expects
ENV PORT 8080

# 5 - Execute
CMD exec gunicorn --bind :$PORT --workers 1 --threads 8 app:app
