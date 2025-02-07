# FastAPI TensorFlow Serving

![Python](https://img.shields.io/badge/Python-3.12-4B8BBE.svg?style=flat&logo=python&logoColor=FFD43B&labelColor=306998)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.18-FF7400.svg?style=flat&logo=tensorflow&logoColor=FF7400&labelColor=212121)](https://www.tensorflow.org/guide)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.115-009688.svg?style=flat&logo=FastAPI&logoColor=009688&labelColor=212121)](https://fastapi.tiangolo.com/tutorial/)
[![uv](https://img.shields.io/badge/astral/uv-261230?style=flat&logo=uv&logoColor=DE5FE9&labelColor=261230)](https://docs.astral.sh/uv/getting-started/installation/)
[![Docker](https://img.shields.io/badge/Docker-329DEE?style=flat&logo=docker&logoColor=white&labelColor=329DEE)](https://docs.docker.com/get-docker/)

![License](https://img.shields.io/badge/license-CC--BY--SA--4.0-31393F?style=flat&logo=creativecommons&logoColor=black&labelColor=white)

GitHub project for Tensorflow-based Object Detection on the CIFAR-10 dataset, served with FastAPI.


## Getting Started

**1.** Install dependencies from pyproject.toml and activate the created virtualenv:
```shell
uv sync && source .venv/bin/activate
```

**2.** Start the app with `gunicorn` with:
```shell
make run
```

**3.** Access the Swagger UI at:
```shell
open http://localhost:8080
```

## Containerization

**1.** Build the Docker Image with:
```shell
make docker-image
```

**2.** Spin up the container with:
```shell
make docker-run
```

**3.** Access the Swagger UI at:
```
open http://localhost:8000
```

## TODO's:
- [x] PEP-517: Packaging and dependency management with `uv`
- [x] Code format/lint with Ruff
- [x] Run on Docker
- [ ] Serve it with Streamlit
- [ ] GitHub CI