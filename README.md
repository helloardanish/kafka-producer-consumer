# kafka-producer-consumer

kafka producer consumer service running on docker/local

## Running on docker

#### Step1: Clone into your local system

```
git clone <link>
```

#### Step 2: Build docker

```
Docker build -t kafka-service:v1 .
```

#### Step 3: Run docker in detached mode

###### Else it will be running in terminal and won't be able to exectue other command in same shell

```
docker run -d kafka-service:v1
```

#### Step 4: Access terminal of docker machine

```
# check the running container
docker ps

# pensive_torvalds is the name of the docker container
docker exec -it pensive_torvalds /bin/bash
```

#### Step 6: Execute the below command in the same path on terminal

```
# run zookeeper
nohup kafka-3.7.0-src/bin/zookeeper-server-start.sh kafka-3.7.0-src/config/zookeeper.properties &

# press enter if nor returned to terminal

# run kafka
nohup kafka-3.7.0-src/bin/kafka-server-start.sh kafka-3.7.0-src/config/server.properties &

# press enter if nor returned to terminal

```

#### Step 7: Run your kafka commands

##### Kafka service is up and running. Run your kafka commands or service it should work

## A R
