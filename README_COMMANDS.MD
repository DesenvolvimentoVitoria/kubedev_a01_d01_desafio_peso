docker image build -t desenvolvimentovitoria/conversao-peso:v1 .
docker container run -d -p 8081:80 --name conversao-peso desenvolvimentovitoria/conversao-peso:v1
docker tag desenvolvimentovitoria/conversao-peso:v1 desenvolvimentovitoria/conversao-peso:latest
docker push desenvolvimentovitoria/conversao-peso:v1
docker push desenvolvimentovitoria/conversao-peso:latest