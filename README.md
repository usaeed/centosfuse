# Cleaning existing image

# Delete all containers
docker rm -f $(docker ps -a -q)
# Delete all images
docker rmi -f $(docker images -q)

# Pre-requisite 
Copy jboss-fuse-full-6.2.0.redhat-133.zip to C:\docker\resources in your windows 7 laptop

# Add the below line in Dockerfile
COPY \resources /tmp
