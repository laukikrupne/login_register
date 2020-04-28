FROM python:3
WORKDIR /usr/src/app
COPY requirements.txt .
RUN sudo apt-get install mysql-client
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
CMD ["python","app.py"]
