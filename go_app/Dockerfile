FROM golang:1.18.3-stretch

WORKDIR /usr/src/app

ENV PATH="/go/bin:${PATH}"
ENV CGO_ENABLED=0

COPY . .

RUN go mod init main.go && go mod tidy

RUN go build -o /docker-gs-ping

CMD [ "/docker-gs-ping" ]
#CMD ["tail", "-f", "/dev/null"]