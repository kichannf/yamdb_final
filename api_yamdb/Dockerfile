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
RUN pwd
RUN ls
RUN pip3 install -r api_yamdb/requirements.txt --no-cache-dir
RUN pwd
RUN ls
CMD ["gunicorn", "api_yamdb.api_yamdb.wsgi:application", "--bind", "0:8000" ] 