FROM python:3.9-buster

WORKDIR /root

RUN pip install --upgrade pip && \
    pip install -U jetson-stats prometheus-client

COPY ./src/jetson_stats_collector.py /root/

ENTRYPOINT ["python3", "jetson_stats_collector.py"]
