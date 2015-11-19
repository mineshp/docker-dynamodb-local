# docker-dynamodb-local

# Build docker container
docker build -t dynamodb-local .

# Run docker app
docker run --name dynamodb-local -P -it --rm dynamodb-local

# Check the docker host port
docker ps

# Get IP address of the VM your docker app is running on
docker-machine ip default

# Access dynamodb local shell in the browser
<IP Address>:<MappedPort>/shell