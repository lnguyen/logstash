# Elastic Search and Logstash Dockerfile

A Dockerfile that produces a Docker Image for [Logstash](logstash.net) and [ElasticSearch](https://www.elastic.co/).


## Usage

### Build the image

To create the image `lnguyen/logstash`, execute the following command on the `logstash` folder:

```
$ docker build -t lnguyen/logstash .
```

### Run the image

To run the image and bind to host port 514, 9200, 9300:

```
$ docker run -d --name logstash -p 514:514 -p 9200:9200 -p 9300:9300 lnguyen/logstash
```
