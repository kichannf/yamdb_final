FROM python:3.7-slim
WORKDIR /app
COPY . .
RUN pip3 install -r api_yamdb/requirements.txt --no-cache-dir
WORKDIR /app/api_yamdb
RUN pwd
RUN ls
CMD ["gunicorn", "api_yamdb.wsgi:application", "--bind", "0.0.0.0:8000" ] 
