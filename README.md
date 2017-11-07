# MAD - Basic Python Webservice Setup

## General Remarks
I decided to use [Flask-RESTful](http://flask-restful.readthedocs.io/en/latest/) as framework to build our REST-APIs. It seems to be suitable for our case.

## Structure
- docker/: All files that are needed to deploy the webservice as docker container
- src: Python file for starting the Flask-RESTful-Server
    - resources/: All resources that are offered by the REST-API
    - ...

## Deploying the Server
To deploy the server just clone [this repo](https://github.com/juliangruendner/mlService_webserviceBase/) and change to the [docker-dirctory](docker/) and execute the command 
``` docker-compose up ``` 
in your terminal. The server will then be reachable on port 5000.

## Extending the API
If you want to extend the functionality of the server just create a new resource in the [resources-directory](src/resources/). Then import the new resource in the [API-file](src/api.py) and add the resource to the *api*-object by using the *add_resource*-function.