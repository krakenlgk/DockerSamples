FROM ubuntu

WORKDIR /app

COPY devops /app

RUN apt-get update && \
    apt-get install -y python3 python3-pip && \
    cd devops

ENTRYPOINT [ "python3" ]
CMD ["manage.py", "runserver", "0.0.0.0:8000"]