[![Docker Build Statu](https://img.shields.io/docker/build/anderkonzen/docker-rails.svg)](https://hub.docker.com/r/anderkonzen/docker-rails/builds/) [![License](http://img.shields.io/:license-mit-blue.svg)](http://doge.mit-license.org)

# Docker Rails

This repo contains **Dockerfiles** for different Ruby and Rails versions.

## Use Cases

These images can be used to bootstrap a new Rails app, or to do any other kind of experiment where you need Rails installed.

For example, to bootstrap a new Rails app in the current folder you can do the following:

```bash
docker run -it --rm -v "$PWD":/app -w /app anderkonzen/rails:5.1.1 new --skip-bundle --force --database=postgresql .
```

## Directory Structure

You might wonder why there is a specific directory for 5.1.1 if in the future I might want to build other versions. Well, I'm using the automated builds from Docker Hub, where I can specify which directories to be monitored. For now it seems a good solution.
