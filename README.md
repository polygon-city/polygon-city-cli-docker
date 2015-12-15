# Polygon City CLI Docker Container

This is a work-in-progress Docker container for setting up and managing the Polygon City CLI. Something like this could be used to easily get the CLI set up and running on a remote server in a self-contained manner instead of running things locally.


## Getting started

```
$ docker-compose build
$ docker-compose up -d
$ docker-compose run node polygon-city [...]
```

## Issues and limitations

* CityGML and output files have to be within the Docker container for now
* Need to work out the best approach for passing in and handling a CityGML file to the Docker container (a volume on the host/local machine?)
* Likewise, need to work out an approach to handle and pass out the resulting output files (a volume on the host/local machine?)
* Unsure if the Redis persistence is working (volume is set up but not sure if it's correct)
