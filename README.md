# mysql-docker-compose
A [docker-compose](https://docs.docker.com/compose/) sample to start `Mysql` database.


# How to use?

1. Clone the project:

  ```shell
    $ git clone https://github.com/gaoshanyu/mysql-docker-compose.git
  ```

2. Start `Mysql` via [docker-compose](https://docs.docker.com/compose/) in terminal:

  ```shell
    $ cd ./mysql-docker-compose
    $ docker-compose up -d
  ```

3. Connect to the Redis server:

  ```shell
    # Enter in the docker container
    $ docker exec -it mysql bash
    # Connect to mysql service, and enter in password 12345678
    $ mysql -h 127.0.0.1 -u root -P 3306 -p
  ```

4. Other commands maybe needed:
  ```shell
    # you can stop service by the command
    $ docker stop mysql
    # you can start service by the command
    # maybe you need this command after your computer restart
    $ docker start mysql
    # you can restart service by the command
    # maybe you need this command after you made some update for [redis.conf]
    $ docker restart mysql
  ```
