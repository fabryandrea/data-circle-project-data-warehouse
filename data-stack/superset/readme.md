
Follow these steps:
- run on your terminal: git clone https://github.com/apache/superset.git
- edit docker-compose-non-dev.yml by changing the image name to: x-superset-image: &superset-image apache/superset:2.1.0
- run on your terminal:  docker-compose -f docker-compose-non-dev.yml pull
- run on your terminal: docker-compose -f docker-compose-non-dev.yml up -d
- run on your terminal: docker exec -it superset_app bash  ./docker/docker-init.sh
- go to http://localhost:8088 and log in by user: admin and pass:admin
