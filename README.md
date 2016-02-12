# Cleaning existing image

# Delete all containers
docker rm -f $(docker ps -a -q)
# Delete all images
docker rmi -f $(docker images -q)

# Pre-requisite 
Copy jboss-fuse-full-6.2.0.redhat-133.zip to C:\docker\resources in your windows 7 laptop

# Clone this repo to c:\docker\ in your windows 7 laptop
git clone URL
cd c:\docker\centosfuse

# Run Docker Quick Start Terminal 
choose start.sh script when prompted
cd c:\docker\centosfuse

# Build
docker build -t shark .
docker images
docker run -i -t shark /bin/bash

# Docker image shark will have bash, java and ps running  
ps -aux 
cd /opt/fuse/jboss-fuse-full-6.2.0.redhat-133/bin
./client -u admin -p admin 

!weldone you are now connected to fuse docker image
