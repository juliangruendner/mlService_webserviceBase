FROM python:3

RUN git clone https://github.com/juliangruendner/mlService_webserviceBase.git
    
    
CMD cd mlService_webserviceBase && \
    git pull && \
    cd docker && \
    chmod +x ./start.sh && \
    ./start.sh