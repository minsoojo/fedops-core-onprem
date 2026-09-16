ARG BASE_IMAGE=docker.io/library/python@sha256:da5aee29682d12a6649f51c8d6f15b87deb3e6c524b923c41d0cb3304d07c913
FROM ${BASE_IMAGE}
WORKDIR /build
COPY . .
RUN python -m pip install --no-cache-dir wheel==0.45.1 && python setup.py bdist_wheel --dist-dir /artifacts
