FROM alpine:latest

RUN apk update && apk add curl nodejs git openjdk17-jdk build-base && curl https://get.gptscript.ai/install.sh | sh && mkdir /.cache /workspace && chmod 777 /.cache /workspace

COPY --from=golang:alpine /usr/local/go/ /usr/local/go/

CMD ["gptscript", "--ui", "--ports=8080-8080"]

WORKDIR /workspace

EXPOSE 8080

ENV PATH="/usr/local/go/bin:${PATH}"
