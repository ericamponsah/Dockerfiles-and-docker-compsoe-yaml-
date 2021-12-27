FROM python:3.6

RUN mkdir /app
WORKDIR /app

COPY requirements.txt /app/
RUN pip install -r requirements.txt

COPY . /app/

EXPOSE 3001

CMD ["python3.6", "front.py"]
