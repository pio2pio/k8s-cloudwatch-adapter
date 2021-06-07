all: clean build ; 
build:
	go build -o ./bin/producer ./producer/main.go
	go build -o ./bin/consumer ./consumer/main.go
clean:
	go clean && rm -rf ./bin
consumer-container:
	docker build -t pio2pio/sqs-consumer-sample ./consumer
producer-container:
	docker build -t pio2pio/sqs-producer-sample ./producer
