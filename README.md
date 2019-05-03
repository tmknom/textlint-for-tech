# textlint-for-tech

[![CircleCI](https://circleci.com/gh/tmknom/textlint-for-tech.svg?style=svg)](https://circleci.com/gh/tmknom/textlint-for-tech)
[![Docker Build Status](https://img.shields.io/docker/cloud/build/tmknom/textlint-for-tech.svg)](https://hub.docker.com/r/tmknom/textlint-for-tech/builds/)
[![Docker Automated build](https://img.shields.io/docker/cloud/automated/tmknom/textlint-for-tech.svg)](https://hub.docker.com/r/tmknom/textlint-for-tech/)
[![MicroBadger Size](https://img.shields.io/microbadger/image-size/tmknom/textlint-for-tech.svg)](https://microbadger.com/images/tmknom/textlint-for-tech)
[![MicroBadger Layers](https://img.shields.io/microbadger/layers/tmknom/textlint-for-tech.svg)](https://microbadger.com/images/tmknom/textlint-for-tech)
[![License](https://img.shields.io/github/license/tmknom/textlint-for-tech.svg)](https://opensource.org/licenses/Apache-2.0)

The pluggable natural language linter for technical writing.

This is [textlint](https://github.com/textlint/textlint) wrapper.

## Requirements

- [Docker](https://www.docker.com/)

## Usage

### Lint markdown

```sh
docker run --rm -v "$PWD:/work" tmknom/textlint-for-tech --config .textlintrc **/*.md
```

### Lint review

```sh
docker run --rm -v "$PWD:/work" tmknom/textlint-for-tech --config .textlintrc **/*.re
```

### Help

```sh
docker run --rm tmknom/textlint-for-tech --help
```

## Makefile targets

```text
build                          Build docker image
format                         Format code
help                           Show help
install                        Install requirements
lint                           Lint code
```

## Development

### Installation

```shell
git clone git@github.com:tmknom/textlint-for-tech.git
cd textlint-for-tech
make install
```

### Deployment

Automatically deployed by "[DockerHub Automated Build](https://docs.docker.com/docker-hub/builds/)" after merge.

### Deployment Pipeline

1. GitHub - Version Control System
   - <https://github.com/tmknom/textlint-for-tech>
2. CircleCI - Continuous Integration
   - <https://circleci.com/gh/tmknom/textlint-for-tech>
3. Docker Hub - Docker Registry
   - <https://hub.docker.com/r/tmknom/textlint-for-tech>
4. MicroBadger - Docker Inspection
   - <https://microbadger.com/images/tmknom/textlint-for-tech>

## License

Apache 2 Licensed. See LICENSE for full details.
