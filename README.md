Using Grpc (https://ewanvalentine.io/microservices-in-golang-part-1/, https://ewanvalentine.io/microservices-in-golang-part-2/)

1. export GOPATH to this Directory.

2. Depedency
go get -u google.golang.org/grpc
go get -u github.com/golang/protobuf/protoc-gen-go

3. Build
cd src/github.com/consignment-service/
make build
make run

4. Testing
cd consignment-cli
go run cli.go

5. Output
2018/07/12 15:13:36 Created: true
2018/07/12 15:13:36 description:"This is a test consignment" weight:550 containers:<customer_id:"naman" origin:"Manchester, United Kingdom" user_id:"user001" > vessel_id:"vessel001"

6. Stop Service
docker ps
docker stop <container id>