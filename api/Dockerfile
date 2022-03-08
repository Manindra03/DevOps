FROM python:3.6.10

RUN mkdir -p /app
WORKDIR /app


COPY requirements.txt app.py /app
RUN pip install flask flask_cors psutil
RUN pip install -r requirements.txt

ENTRYPOINT [ "flask" ]
CMD ["run", "--host=0.0.0.0", "--port=5000"]