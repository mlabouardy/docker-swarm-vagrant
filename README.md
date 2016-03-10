# Create Token

docker run swarm create

# Create Cluster manager

docker run -d -P swarm manage token://TOKEN

# Join Cluster

docker run -d -P swarm join --addr=IP:2375 token://TOKEN

# Show info

docker -H tcp://IP:PORT info

# List nodes

docker run swarm list token://TOKEN
