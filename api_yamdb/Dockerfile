FROM python:3.7-slim
WORKDIR /app
COPY . /app
RUN python -m pip install --upgrade pip
RUN python -m pip install -r requirements.txt --no-cache-dir
CMD ["gunicorn", "api_yamdb.wsgi:application", "--bind", "0:8000" ]
