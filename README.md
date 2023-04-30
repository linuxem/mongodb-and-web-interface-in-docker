# mongodb-and-web-interface-in-docker

MongoDB: just on your machine run the Docker Pull command

``` docker pull mongo ```

Create MongoDB Database Server Container

``` sudo mkdir /var/dbdata ```

Now, Run Mongo Container:

``` docker run -it -d -v /var/dbdata:/data/db -p 27017:27017 --name mongodb mongo ```

Start container:

``` docker start mongodb ```

Access MongoDB Database Docker Terminal (Bash Shell)


``` sudo docker exec -it mongodb bash ```


 