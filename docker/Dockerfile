FROM us.gcr.io/grafeas/grafeas-server:v0.1.0
WORKDIR /
COPY ./server/wait.sh /wait.sh
COPY ./server/start.sh /start.sh
EXPOSE 8080

ENTRYPOINT ["./start.sh"]
