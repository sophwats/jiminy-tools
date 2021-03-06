# predictor-mock

This is a mock predictor server to help with testing scenarios.

## Quickstart

The easiest way to utilize these modules for loading a database is by
creating a virtual environment using the
[virtualenv](https://pypi.python.org/pypi/virtualenv) tool.

after activating the virtual environment, you will need to install the
requirements for this tool by running the following:

    pip install -r requirements.txt

to run the server simply start it with the following:

    python app.py

it will now be running on `127.0.0.1:8080`, you may interact with it using
the api defined by
[this openapi definition](https://github.com/radanalyticsio/jiminy-predictor/blob/master/docs/openapi.yaml)

## OpenShift deploy

To run this mock service on OpenShift, simply use the following command:

```
oc new-app centos/python-27-centos7~https://github.com/radanalyticsio/jiminy-tools --context-dir=predictor-mock --name=predictor-mock
```
