docker build -t pqn src/docker
docker container run -p 8888:8888 -v ${PWD}:/project -w /project  -it pqn jupyter lab --allow-root --ip 0.0.0.0