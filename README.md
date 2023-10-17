set Host file:

192.168.88.120 cronicle

copy cronicle.json.import to data/data/

# DOCKER SWARM

docker stack deploy -c cronicle.yml cronicle

docker stack rm cronicle

docker service logs --follow --tail=25 cronicle_cronicle

# docker-cronicle-docker
