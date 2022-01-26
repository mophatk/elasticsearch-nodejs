# Search demo

## Demo

### Starting the demo

This repository includes a Docker Compose file to reproduce the environment locally.

Execute the following commands to start and create the index with sample data:

```bash
docker-compose up
# Wait until the elasticsearch container says "started". Then open a new temrinal and import
# data into the index with the following command:
docker exec elasticsearchnodejs_web_1 /usr/src/app/elasticsearch-data/load-data.sh
```

Finally, open http://localhost:3000 in a browser to see the search page.

### Stopping the demo

Open the terminal where you executed `docker-compose up` and press Ctrl + c, which will
stop the containers. 
