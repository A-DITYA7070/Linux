1. install docker image :- sudo apt install docker.io
2. pull mysql from docker :- sudo docker pull mysql
3. execute mysql :- sudo docker run --name test-mysql -e MYSQL_ROOT_PASSWORD=password123 -d mysql:latest
4. list the container of docker :- sudo docker container ps 
5. Execute the container with container id  :- sudo docker exec -it 32a6252d9c83 bash
6. Login to sql :- bash-5.1# mysql -uroot -ppassword123
