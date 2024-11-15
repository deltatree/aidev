FROM alpine:latest

RUN apk update && url https://get.gptscript.ai/install.sh | sh && mkdir /.cache && chmod 777 /.cache

CMD ["gptscript", "--cache=false", "--ui", "--ports=8080-8080"]

EXPOSE 8080
