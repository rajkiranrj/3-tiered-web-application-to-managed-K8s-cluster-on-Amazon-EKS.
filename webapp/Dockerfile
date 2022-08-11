FROM python:alpine

ADD ./requirements.txt /opt/webapp-mysql/

RUN pip install pip --upgrade

WORKDIR /opt/webapp-mysql

RUN pip install -r requirements.txt

ADD . /opt/webapp-mysql

EXPOSE 81

CMD python /opt/webapp-mysql/app.py
