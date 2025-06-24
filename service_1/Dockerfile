FROM golang:1.18

WORKDIR /app

COPY go.mod ./
RUN go mod download

COPY . ./

RUN go build -o main .

# ✅ Install curl for health checks
RUN apt-get update && apt-get install -y curl

EXPOSE 8001

CMD ["./main"]
