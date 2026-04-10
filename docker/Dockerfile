FROM python:3.10-slim

WORKDIR /app

COPY app/requirements.txt .

RUN pip install --trusted-host pypi.org \
    --trusted-host files.pythonhosted.org \
    -r requirements.txt

COPY app/ .

CMD ["python", "app.py"]