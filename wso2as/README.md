# Dockerfile for WSO2 Application Server #
The Dockerfile defines the resources and instructions to build the Docker images with the WSO2 products and runtime configurations.

## Try it out

The cloned local copy of WSO2 Dockerfiles will be referred as `DOCKERFILES_HOME`.

* Add product packs and dependencies
    - Download and copy JDK 1.7 ([jdk-7u80-linux-x64.tar.gz](http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html)) pack to `<DOCKERFILES_HOME>/common/provision/default/files`.
    - Download the WSO2 Application Server zip file (http://wso2.com/products/application-server/) and copy it to `<DOCKERFILES_HOME>/common/provision/default/files`.

* Build the docker image
    - Navigate to `<DOCKERFILES_HOME>/wso2as`.
    - Execute `build.sh` script and provide the product version.
        + `./build.sh -v 5.3.0`

* Docker run
    - Navigate to `<DOCKERFILES_HOME>/wso2as`.
    - Execute `run.sh` script and provide the product version.
        + `./run.sh -v 5.3.0`

* Access management console
    -  To access the management console, use the docker host IP and port 9443.
        + `https://<DOCKER_HOST_IP>:9443/carbon`

## Detailed Configuration

* [Introduction] (https://docs.wso2.com/display/DF100/Introduction+to+Docker+Images)

* [Building docker images] (https://docs.wso2.com/display/DF100/Building+Product+Docker+Images)

* [Running docker images] (https://docs.wso2.com/display/DF100/Running+and+Migrating+Images)
