- Install Docker:
sudo apt update
sudo apt -y install docker.io
sudo systemctl status docker

- Display Docker Version:
sudo docker version

- Display Docker Info:
sudo docker info

- Verification of Docker:
sudo docker run hello-world

- Display downloaded image:
sudo docker image ls

- Display all container:
sudo docker container ls -a

- Run Image:
sudo docker run [image-name]

- Build image: 
sudo docker build -t [name] .

- Run compose:
sudo docker-compose up -d

- Display active compose:
sudo docker-compose ps

- Display variable env in service:
sudo docker-compose run [service-name] env


