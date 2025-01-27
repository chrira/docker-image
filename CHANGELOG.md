# Changelog

## 2022-09-28

### Changed

- Change base image from `eclipse-temurin:17-jre-focal` to `eclipse-temurin:17-jre-jammy` for images 10.0 and higher.

## 2022-09-05

### Changed

- Change base image from `eclipse-temurin:11-jre-focal` to `eclipse-temurin:17-jre-focal` for images 9.4 and higher.

## 2022-28-01

### Changed

- Change base image from unmaintaned `adoptopenjdk/openjdk11:debianslim-jre` image to maintained `eclipse-temurin:11-jre-focal` image. This changes affects the following versions:
  - LTS 8.0: 8.0.25 and higher
  - Leading Edge 9: 9.3.3 and higher

## 2021-03-11

### Changed

- Axon Ivy Engine Docker image is no longer built on the Axon Ivy Engine Debian package.
  This change affects the following versions:
  - LTS 8.0: 8.0.15 and higher
  - Leading Edge 9: 9.1.1 and higher

- web.xml and context.xml not available in global configuration directory LTS 8.0 (8.0.15 and higher)
  - web.xml must be mounted /usr/lib/axonivy-engine/webapps/ivy/WEB-INF/web.xml
  - context.xml must be mounted /usr/lib/axonivy-engine/webapps/ivy/META-INF/context.xml
