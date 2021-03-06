# Fastapi-lazy 🦥

![lazy](https://user-images.githubusercontent.com/52716203/135530036-3ed731f6-e0db-4de6-8667-9af75656f2f4.png)

<p align="center">
    <em>Utilities that you use in various projects made in FastAPI.</em>
</p>

[![PyPI version](https://badge.fury.io/py/fastapi-lazy.svg)](https://badge.fury.io/py/fastapi-lazy)
[![Downloads](https://pepy.tech/badge/fastapi-lazy/month)](https://pepy.tech/project/fastapi-lazy)
[![Downloads](https://pepy.tech/badge/fastapi-lazy/week)](https://pepy.tech/project/fastapi-lazy)
[![Language](https://img.shields.io/badge/Language-Python-green?style)](https://github.com/yezz123)
[![framework](https://img.shields.io/badge/Framework-FastAPI-blue?style)](https://fastapi.tiangolo.com/)
[![Star Badge](https://img.shields.io/static/v1?label=%F0%9F%8C%9F&message=If%20Useful&style=style=flatcolor=BC4E99)](https://github.com/yezz123/fastapi-lazy)
[![Pypi](https://img.shields.io/pypi/pyversions/fastapi-lazy.svg?color=%2334D058)](https://pypi.org/project/fastapi-lazy)

---

**Source Code**: <https://github.com/yezz123/fastapi-lazy>

**Install the project**: `pip install fastapi-lazy`

---

## Features 🎉

- Use the data contained in the JWT
- Use the username contained in the JWT and fetch data.
- Create User Models based on Pydantic.
- Multi Database Support:
  - Creates the dependency to be used to connect to the Postgresql.
  - Creates the dependency to be used to connect to the MongoDB.
  - Create the dependency to be used to connect to the SQlite using SQLAlchemy.
- Support Redis Cache:
  - Creates a `pickle` of the object passed as a parameter and saves it in the Redis which is also passed as a parameter.
  - Read the `pickle` of the object saved in RedisDB and return it as Python object.
- Support UUID generator:
  - Create a custom UUID4 using the current timestamp.
  - Create a JWT token creator & verifier.
- Create a simple Password hash using `hashlib`.
- Create an Email Validator.
- Provide a Token Creator for login after adding a new package `passlib`.
- Add A simple Crud file for MongoDB Provider.
  - Soon will be added for Postgresql Provider, & SQLite Provider.

## Development 🚧

You should create a virtual environment and activate it:

```bash
python -m venv venv/
```

```bash
source venv/bin/activate
```

And then install the development dependencies:

```bash
pip install -r requirements.dev.txt
```

### Format the code 💅

Execute the following command to apply `pre-commit` formatting:

```bash
make lint
```

## License 🍻

This project is licensed under the terms of the MIT license.
