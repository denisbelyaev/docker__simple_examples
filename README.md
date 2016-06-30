execute:
/example-triggers/ docker build -t denisbelyaev/node_trigger_example .
/example-triggers/app/ docker duild -t denisbelyaev/node_app_example .

docker run -d -p 4567:9000 --name nodeapp denisbelyaev/node_trigger_example

//default docker host ip
ifconfig: docker0:  http://172.17.0.1:4567
