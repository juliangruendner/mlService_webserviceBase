# MAD - Basic Python Webservice Setup

## General Remarks
I decided to use [Flask-RESTful](http://flask-restful.readthedocs.io/en/latest/) as framework to build our REST-APIs. It seems to be suitable for our case.

## Structure
- docker/: All files that are needed to deploy the webservice as docker container
- src: Python file for starting the Flask-RESTful-Server
    - resources/: All resources that are offered by the REST-API
    - ...

## Deploying the Server
To deploy the server 