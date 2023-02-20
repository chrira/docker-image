[![LTS][1]][0] [![Latest][2]][0] 
[![Sprint][3]][0] [![Nightly][4]][0] [![Dev][5]][0]

# Axon Ivy Engine Docker Image

Get an Axon Ivy Engine running with only one command:

    docker run -p 8080:8080 axonivy/axonivy-engine

Open your browser and go to <http://localhost:8080>

We have many [docker-samples](https://github.com/ivy-samples/docker-samples)
to see how Axon Ivy Engine can be used in a docker container.

## Development

Build your Image locally:

```s
VERSION=10.0
ENGINE_URL=https://developer.axonivy.com/permalink/${VERSION}/axonivy-engine.zip
IMAGE=axonivy/axonivy-engine
IMAGE_TAG=${IMAGE}:${VERSION}-local
docker build -t ${IMAGE_TAG} axonivy-engine/${VERSION} --build-arg IVY_ENGINE_DOWNLOAD_URL=${ENGINE_URL}
```

Run your fresh built Image with this command:

```s
docker run -p 8080:8080 ${IMAGE_TAG}
```

## Changelog

See [changelog](CHANGELOG.md) for changes related to the Docker Image.

[0]: https://hub.docker.com/r/axonivy/axonivy-engine/tags
[1]: https://img.shields.io/badge/docker-8.0-green
[2]: https://img.shields.io/badge/docker-latest-yellowgreen
[3]: https://img.shields.io/badge/docker-sprint-yellow
[4]: https://img.shields.io/badge/docker-nightly-orange
[5]: https://img.shields.io/badge/docker-dev-red
