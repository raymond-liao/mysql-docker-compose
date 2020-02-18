# mysql-docker-compose
A [docker-compose](https://docs.docker.com/compose/) sample to start `MySQL` database.


# How to use?

1. Clone the project:

  ```shell
    $ git clone https://github.com/gaoshanyu/mysql-docker-compose.git
  ```

2. Start `MySQL` via [docker-compose](https://docs.docker.com/compose/) in terminal:

  ```shell
    $ cd ./mysql-docker-compose
    // Please add path "/usr/local/var/mysql" as the sharing folder for your Docker before
    $ docker-compose up -d
  ```

3. Connect to the MySQL server:

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
    $ docker start mysql
    # you can restart service by the command
    $ docker restart mysql
  ```
