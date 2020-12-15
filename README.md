# <img src="https://uploads-ssl.webflow.com/5ea5d3315186cf5ec60c3ee4/5edf1c94ce4c859f2b188094_logo.svg" alt="Pip.Services Logo" width="200"> <br/> RESTful client facade for Python

**Important**: This module has been deprecated. Please, use RestOperations from [pip-services3-rpc-python](https://github.com/pip-services3-python/pip-services3-rpc-python) instead.

One of the common implementation patterns is to expose microservices via single entry point called API Gateway or Client Facade.
The responsiblity of that component is to accept calls from external consumers, enforce security rules, perform authentication and authorization
and when request is cleared it can call one or few microservices in a single transaction. Client Facades may also implement complex requests,
combine multiple datasets and return then in a single transaction, push notifications via async mechanisms like Socket.IO or WebSockets.

This module is a part of the [Pip.Services](http://pip.services.org) polyglot microservices toolkit.
It provides reusable primitives to quickly build sophisticated client facades via composition of multiple routes and middleware components.

- **Auth** - Authentication and authorization components
- **Build** - Contains a factory for constructing facade components
- **Container** - Facade launch container
- **Operations** - Basic facade operations called by clients
- **Services** - Main and partition (subpath) facade services
- **Routes** - Abstract facade route class and few generic routes
- **Errors** - Error simulation

<a name="links"></a> Quick links:

* [API Reference](https://pip-services3-python.github.io/pip-services3-facade-python/)
* [Change Log](CHANGELOG.md)
* [Get Help](https://www.pipservices.org/community/help)
* [Contribute](https://www.pipservices.org/community/contribute)


## Use

Get the package from pip
```bash
pip install -U pip-services3-facade
```

## Develop

For development you shall install the following prerequisites:
* Python 3.7+
* Visual Studio Code or another IDE of your choice
* Docker

Install dependencies:
```bash
pip install -r requirements.txt
```

Run automated tests:
```bash
python test.py
```

Generate API documentation:
```bash
./docgen.ps1
```

Before committing changes run dockerized build and test as:
```bash
./build.ps1
./test.ps1
./clear.ps1
```

## Contacts

The Python version of Pip.Services is created and maintained by **Sergey Seroukhov**
