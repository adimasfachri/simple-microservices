.PHONY : build run-docker clean

build:
	docker build -t employee-service-kong .

run-docker:
	docker run -d --rm --name employee-service-kong \
	--network=compose_kong-net \
	-p 8004:8004 \
	employee-service-kong

clean:
	docker rmi -f employee-service-kong
