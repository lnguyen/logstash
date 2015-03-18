# Elastic Search and Logstash Dockerfile

A Dockerfile that produces a Docker Image for [Logstash](logstash.net) and [ElasticSearch](https://www.elastic.co/).


## Usage

### Build the image

To create the image `lnguyen/el`, execute the following command on the `elk` folder:

```
$ docker build -t lnguyen/el .
```

### Run the image

To run the image and bind to host port 514, 9200, 9300:

```
$ docker run -d --name el -p 514:514 -p 9200:9200 -p 9300:9300 lnguyen/el
```
