FROM python:3.10-slim
WORKDIR /client
COPY requirements.txt .
RUN apt-get update && apt-get install -y ffmpeg
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
CMD ["python", "client.py"]