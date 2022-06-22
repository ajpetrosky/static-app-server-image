# syntax=docker/dockerfile:1

FROM golang:1.17-alpine

WORKDIR /app

COPY go.mod ./
RUN go mod download

COPY server.go ./

RUN go build -o /static-server

EXPOSE 8080