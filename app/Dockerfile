FROM python:3.6
  
EXPOSE 5000
  
WORKDIR /app

COPY requirements.txt /app

RUN pip install -r requirements.txt

RUN apt-get -y update

RUN groupadd -r user && useradd -r -g user user

USER prajwal

COPY app.py /app

CMD python app.py
