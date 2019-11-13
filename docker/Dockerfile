FROM us.gcr.io/grafeas/grafeas-server:0.1.0
WORKDIR /
RUN useradd -r -u 8080 grafeas
USER grafeas
COPY ./server/wait.sh /wait.sh
COPY ./server/start.sh /start.sh
EXPOSE 8080

ENTRYPOINT ["./start.sh"]
