# PySpark Notebook

This repository builds on top of Jupyter's [PySpark Notebook](https://github.com/jupyter/docker-stacks/tree/master/pyspark-notebook) Docker image, adding tools to make it even more pratical to use Spark on a local machine without the need to actually download and set it up.

This image is aimed for those people tha want a local and interactive environment to develop a PySpark application, before submitting it to production.

The image also sets up all the configuration needed to connect to Amazon S3 file service, and thus the user can also work with on-cloud data. That being said, the user must set the AWS-related variables in a .env file to access this functionality.

## Dependecies

* Docker >= 20.10.8
* Docker-Compose >= 1.29.2

Although previous versions were not tested, it is posible that they work.

## Quick Start

All you have to do is to properly set up environment variables and the python packages your project depends on, through the `.env` and `requirements.txt` files, respectively.

The project contains templates of these files that you should edit before trying to start the Docker container.

After that, just run thw following command in the folder that contains the files:

```
docker compose up -d
```

A jupyter lab application should be available at `localhost:8888`.

## Author
Created by Pedro Toledo. Feel free to contact me!

[![Twitter Badge](https://img.shields.io/badge/-@pedrotol_-1ca0f1?style=flat-square&labelColor=1ca0f1&logo=twitter&logoColor=white&link=https://twitter.com/pedrotol_)](https://twitter.com/pedrotol_)
[![Linkedin Badge](https://img.shields.io/badge/-Pedro_Toledo-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/pedro-toledo/)](https://www.linkedin.com/in/pedro-toledo/)
[![Gmail Badge](https://img.shields.io/badge/-pedroltoledo@gmail.com-c14438?style=flat-square&logo=Gmail&logoColor=white&link=mailto:tgmarinho@gmail.com)](mailto:pedroltoledo@gmail.com)