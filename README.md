Using Grpc (https://ewanvalentine.io/microservices-in-golang-part-1/, https://ewanvalentine.io/microservices-in-golang-part-2/)<Br>
<Br>
1. export GOPATH to this Clone Directory.<Br>
<Br>
2. Depedency<Br>
go get -u google.golang.org/grpc<Br>
go get -u github.com/golang/protobuf/protoc-gen-go<Br>
<Br>
3. Build<Br>
cd src/github.com/consignment-service/<Br>
make build<Br>
make run<Br>
<Br>
4. Testing<Br>
cd consignment-cli<Br>
go run cli.go<Br>
<Br>
5. Output<Br>
2018/07/12 15:13:36 Created: true<Br>
2018/07/12 15:13:36 description:"This is a test consignment" weight:550 containers:<customer_id:"naman" origin:"Manchester, United Kingdom" user_id:"user001" > vessel_id:"vessel001"<Br>
<Br>
6. Stop Service<Br>
docker ps<Br>
docker stop <container id><Br>