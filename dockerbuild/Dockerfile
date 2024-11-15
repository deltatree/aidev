FROM alpine:latest

RUN apk update && apk add curl && curl https://get.gptscript.ai/install.sh | sh && mkdir /.cache && chmod 777 /.cache

CMD ["gptscript", "--ui", "--ports=8080-8080"]

EXPOSE 8080
