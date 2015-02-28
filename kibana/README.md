# kibana 4 in docker

This is dockerized version of [kibana 4](https://github.com/elasticsearch/kibana).

## Build your image

```
  docker build -t weij/kibana .
```

## Running

```
docker run -d -p <host ip>:<host port>:5601 -e KIBANA_ES_URL=<elasticsearch url>  weij/kibana4
```
eg. docker run -d -p 5601:5601 -e KIBANA_ES_URL=http://192.168.59.103:9200  weij/kibana4