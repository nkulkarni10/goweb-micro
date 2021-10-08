FROM golang:alpine

# Set necessary environmet variables needed for our image
ENV GO111MODULE=on \
    CGO_ENABLED=0 \
    GOOS=linux

WORKDIR /code

COPY . .

#WORKDIR /code/goweb_microservices/admin_microservice/ad_microservice/admin_microservice

#WORKDIR /code/admin_microservice

#RUN go build -o admin_microservice .

#WORKDIR /code/login_microservice

#RUN go build -o login_microservice .

WORKDIR /code/grpc_server

RUN go build -o grpc_server .

#CMD ["./admin_microservice"]
#CMD ["./login_microservice"]
CMD ["./grpc_server"]