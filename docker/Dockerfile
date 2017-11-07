FROM python:3

COPY start.sh /
COPY requirements.txt /

RUN chmod +x ./start.sh

RUN pip3 install -r requirements.txt && \
    git clone https://github.com/juliangruendner/mlService_webserviceBase.git

ENTRYPOINT ./start.sh