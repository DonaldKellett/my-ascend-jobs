FROM harbor.internal.donaldsebleung.com/ascendhub/mindspore:2.10.0-cann8.5.0-310p-openeuler24.03-py3.11.post1
WORKDIR /app
COPY main.py .
VOLUME /app/work
WORKDIR /app/work
CMD [ \
    "msrun", \
    "--worker_num=2", \
    "--local_worker_num=2", \
    "--join=True", \
    "python", \
    "/app/main.py" \
]
