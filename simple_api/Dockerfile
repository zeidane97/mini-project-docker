FROM python:2.7-stretch

RUN mkdir /data
COPY student_age* /data/
RUN apt-get  update -y && apt-get  install python-dev python3-dev libsasl2-dev python-dev libldap2-dev libssl-dev -y
RUN pip install flask==1.1.2 flask_httpauth==4.1.0 flask_simpleldap python-dotenv==0.15

VOLUME /data

EXPOSE 5000
CMD [ "python", "./data/student_age.py" ]
MAINTAINER Zeidane

