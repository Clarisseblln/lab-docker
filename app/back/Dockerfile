FROM python:3.13-slim
 
WORKDIR /app
 
COPY requirements.txt .
 
RUN pip install --no-cache-dir -r requirements.txt
 
COPY . .
 
ENV FLASK_APP=app.py
 
CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0"]