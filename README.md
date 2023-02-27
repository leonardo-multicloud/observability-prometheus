# observability-prometheus

docker build -t leonardomulticloud/go_app:latest -f .\go_app\Dockerfile . --no-cache
docker-compose up -d
docker exec -it app bash