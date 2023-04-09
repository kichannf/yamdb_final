FROM python:3.7-slim
# # COPY ./ /app
# # RUN pip3 install -r /app/api_yamdb/requirements.txt --no-cache-dir
# # WORKDIR /app/api_yamdb/
# RUN pwd
# RUN ls
# WORKDIR /app
# RUN pwd
# RUN ls
# COPY . .
# RUN pwd
# RUN ls
# RUN pip3 install -r api_yamdb/requirements.txt --no-cache-dir
# WORKDIR /app/api_yamdb
# RUN pwd
# RUN ls
WORKDIR /app
COPY . .
RUN pip3 install -r requirements.txt --no-cache-dir
WORKDIR /app/api_yamdb/api_yamdb
CMD ["gunicorn", "wsgi:application", "--bind", "0:8000" ] 