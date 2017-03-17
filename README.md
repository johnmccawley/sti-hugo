# Hugo Docker Images

This is an source builder image for [Hugo](http://www.gohugo.io) - a fast and modern static web site generator.

This repository contains the source for building various versions of the Hugo static site generator as a reproducible Docker image using source-to-image. This image uses the Alpine Linux distribution. The resulting image can be run using Docker.

For more information about using these images with Digital Garage on OpenShift and Kubernetes, please see the official Digital Garage Documentation.

## Versions

Hugo versions currently provided are:

GoLang 1.8-alpine
Hugo v0.19

## How to use this image on Digital Garage with OpenShift and Kubernetes?

Run:

```
$ oc new-app thedigitalgarage/sti-hugo019-alpine~http://github.com/<org>/<hugo-repo>
```

## Usage

For information about usage of Dockerfile for Hugo v0.19, see usage documentation.

## Repository organization

<hugo-version>

Dockerfile and scripts to build container images from.

hack/

Folder containing scripts which are responsible for the build and test actions performed by the Makefile.

Image name structure

Structure: thedigitalgarage/sti-1-2-3

Platform name (lowercase) - hugo
Platform version(without dots) - 019
Base builder image - alpine
Examples: thedigitalgarage/sti-hugo019-alpine
