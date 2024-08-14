FROM python:3.8-buster
MAINTAINER siega
ADD student_age.py /
ADD requirements.txt /
RUN apt update -y 
RUN apt install python-dev python3-dev libsasl2-dev python-dev libldap2-dev libssl-dev -y
RUN pip3 install -r ./requirements.txt
VOLUME /data
EXPOSE 5000
CMD [ "python3", "./student_age.py" ]