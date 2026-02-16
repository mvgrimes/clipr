FROM alpine

RUN adduser -S -D -H -h /app appuser
WORKDIR /app

COPY ./clip-linux-amd64 /app/clip
RUN chmod +x /app/clip

USER appuser

EXPOSE 8080
CMD [ "/app/clip", "server" ]
