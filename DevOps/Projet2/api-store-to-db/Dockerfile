FROM python:alpine

ADD __main__.py /root
ADD _version.py /root
ADD requirements.txt /root

RUN pip install -r /root/requirements.txt

EXPOSE 80

CMD [ "python", "/root/__main__.py", "-Aapi-bracelet", , "-Hapi-bracelet-mongodb", "-Dbracelet" ]