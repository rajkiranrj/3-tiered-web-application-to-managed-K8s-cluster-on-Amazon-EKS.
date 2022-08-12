FROM python:alpine

RUN pip install --upgrade pip

ADD ./requirements.txt /opt/webapp-mysql/

WORKDIR /opt/webapp-mysql

RUN pip install -r requirements.txt

ADD . /opt/webapp-mysql

EXPOSE 81

CMD python /opt/webapp-mysql/app.py
