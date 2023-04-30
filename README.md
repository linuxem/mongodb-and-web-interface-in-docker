# mongodb-and-web-interface-in-docker

MongoDB: just on your machine run the Docker Pull command

``` docker pull mongo ```

Create MongoDB Database Server Container

``` mkdir dbdata ```

Now, Run Mongo Container:

``` docker run -it -d -v dbdata:/data/db -p 27017:27017 --name mongodb mongo ```

Start container:

``` docker start mongodb ```

Access MongoDB Database Docker Terminal (Bash)


``` docker exec -it mongodb bash ```


Create Mongo Express Web Interface container (optional)

``` docker run --link mongo_db_name_container:mongo -p 8081:8081 -e ME_CONFIG_MONGODB_URL="mongodb://mongo:27017" mongo-express ```

