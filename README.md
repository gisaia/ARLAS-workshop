# ARLAS-workshop

The workshop's aim is to present ARLAS's capabilities to explore big volumes of geo-spatial data using an analytic and geo-analytic approach.


The first part of the workshop will be a global presentation of the solution and different use cases in which it is used, and then a technical presentation.

In the second part, we will explore data of :

- Boats navigating around the Dannish sea
- OpenStreetMap buildings with a geo-analytic perspective
- Air pollution around the globe

These examples will help you go through the different steps to start exploring data with ARLAS :
- Studying the data and make it analytics ready
- Starting the ARLAS-stack and reference the data in ARLAS
- Building dashboards with map layers and widgets
- Exploring the data.


## Prepare the workshop:

- The workshop is prepared to be run under Linux / Mac OSX operating system.
- You will need to have `docker` and `docker-compose` installed
- You will need `curl` for http requests and to download some tools for the workshop

- You can already pull the docker images used in the tutorial

    ARLAS stack images:
    ```shell
    docker pull gisaia/arlas-wui:18.1.1
    docker pull gisaia/arlas-wui-builder:18.1.1
    docker pull gisaia/arlas-wui-hub:18.1.0
    docker pull gisaia/arlas-server:18.7.1
    docker pull gisaia/arlas-persistence-server:18.0.0
    ```

    Elasticsearch image:
    ```
    docker pull docker.elastic.co/elasticsearch/elasticsearch:7.9.2
    ```

- You will also need to install logstash to ingest data in Elasticsearch
    ```
    curl https://raw.githubusercontent.com/gisaia/ARLAS-stack-ais-tutorial/develop/configs/ais2es.logstash.conf -o ais2es.logstash.conf
    ```