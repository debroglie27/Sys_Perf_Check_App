FROM python:3.8
WORKDIR /app
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
CMD ["python3", "client_end_script.py", "-l", "10", "-u", "30", "-s", "10", "-t", "20"]
