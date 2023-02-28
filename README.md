
  # Personal Things 

This project is for personal investigations if you find any use in this, excellent!.

### Set up the environment

1. Install [Poetry](https://python-poetry.org/docs/#installation)

2. Set up the environment:

```bash
make setup
make activate
```

### Install new packages

To install new PyPI packages, run:

```bash
poetry add <package-name>
```


### Run Python scripts

To run the Python scripts to process data, train model, and run a notebook, type the following:

```bash
make pipeline
```

### View all flow runs

A [flow](https://docs.prefect.io/concepts/flows/) is the basis of all Prefect workflows.

  
To view your flow runs from a UI, sign in to your [Prefect Cloud](https://app.prefect.cloud/) account or spin up a Prefect Orion server on your local machine:

```bash

prefect orion start

```

Open the URL http://127.0.0.1:4200/, and you should see the Prefect UI:

![](images/prefect_cloud.png)

  
### Run flows from the UI

After [creating a deployment](https://towardsdatascience.com/build-a-full-stack-ml-application-with-pydantic-and-prefect-915f00fe0c62?sk=b1f8c5cb53a6a9d7f48d66fa778e9cf0), you can run a flow from the UI with default parameters:

API documentation

To auto-generate API document for your project, run:



```bash

make docs_save

```


### Run tests when creating a PR

When creating a PR, the tests in your `tests` folder will automatically run.
