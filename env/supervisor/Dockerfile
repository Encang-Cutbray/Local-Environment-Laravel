FROM larahouse/phpfpm:7.4

RUN apt-get update && apt-get install -y nano supervisor

# Create Supervisor log
RUN mkdir -p /var/log/supervisor

EXPOSE 6060

COPY supervisord.conf /etc/supervisor/supervisord.conf
ENTRYPOINT ["/usr/bin/supervisord", "-n", "-c",  "/etc/supervisor/supervisord.conf"]


