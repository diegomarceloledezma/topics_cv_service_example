# topics_cv_service_example

This is an example repo for deploying a computer vision model as a web service.

## Installation
Create a virtual environment for the project:

### Anaconda/miniconda

```
conda create -n web_cv python=3.11
conda activate web_cv
```

Install the dependencies:

```
pip install -r requirements.txt
pip install -r requirements-dev.txt
```

### UV

```
uv init
uv sync --frozen
```

## Running locally

Once dependencies are installed, activate the virtual environment and run:

```
fastapi dev src/main.py
```

Then, go to http://localhost:8000/docs for interacting with the API

## Using Docker

You can run this service using docker and docker compose:

```
docker compose up --build
```

Then, go to http://localhost:8000/docs for interacting with the API

## Formatting the code
In order to keep the code clean, you can check the formating of the code:

```
ruff check
```

## Running tests
You can launch the test suite with pytest:

```
pytest tests
```