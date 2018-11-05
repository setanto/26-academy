FROM python:alpine


ARG APIHOST
ARG MONGOHOST
ARG MONGODB
ARG MONGOUSER
ARG MONGOPASSWORD

ADD __main__.py /root
ADD _version.py /root
ADD requirements.txt /root

RUN pip install -r /root/requirements.txt

EXPOSE 80

CMD [ "python", "/root/__main__.py", "-A$APIHOST", "-H${MONGOHOST}", "-D${MONGODB}", "-u${MONGOUSER}", "-p${MONGOPASSWORD}" ]