Glide Docker Image
==================

[![GitHub release](https://img.shields.io/github/release/instrumentisto/glide-docker-image.svg)](https://hub.docker.com/r/instrumentisto/glide/tags) [![Build Status](https://travis-ci.org/instrumentisto/glide-docker-image.svg?branch=master)](https://travis-ci.org/instrumentisto/glide-docker-image) [![Docker Pulls](https://img.shields.io/docker/pulls/instrumentisto/glide.svg)](https://hub.docker.com/r/instrumentisto/glide)




## What is Glide?

Glide is a tool for managing the `vendor` directory within a Go package. This feature, first introduced in Go 1.5, allows each package to have a `vendor` directory containing dependent packages for the project. These vendor packages can be installed by a tool (e.g. `glide`), similar to `go get` or they can be vendored and distributed with the package.

Are you used to tools such as Cargo, npm, Composer, Nuget, Pip, Maven, Bundler, or other modern package managers? If so, Glide is the comparable Go tool.

> [glide.sh](https://glide.sh)

![Glide Logo](https://glide.sh/assets/logo-small.png)




## How to use this image

Mount your project into correct `$GOPATH` directory and provide the `glide` command you require:

```bash
docker run --rm -it -v $(pwd):/go/src/my/pkg/name -w /go/src/my/pkg/name \
    instrumentisto/glide install
```




## Image versions


### `latest`

Latest version of Glide on latest Golang version.


### `X.Y`

Latest version of Glide `X.Y` branch on latest Golang version.


### `X.Y.Z`

Concrete `X.Y.Z` version of Glide on latest Golang version.


### `X.Y.Z-goA.B`

Concrete `X.Y.Z` version of Glide on latest Golang `A.B` version.




## License

Glide itself is licensed under [MIT license][91].

And Glide Docker image is licensed under [MIT license][92] too.




## Issues

We can't notice comments in the DockerHub, so don't use them for reporting issue or asking question.

If you have any problems with or questions about this image, please contact us through a [GitHub issue][10].





[10]: https://github.com/instrumentisto/glide-docker-image/issues
[91]: https://github.com/Masterminds/glide/blob/master/LICENSE
[92]: https://github.com/instrumentisto/glide-docker-image/blob/master/LICENSE.md
