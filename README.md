# DARPA-ASKEM.github.io
Documentation site for the DARPA-ASKEM Organization

## Developing

We recommend running Jekyll in Docker to build the docs locally for editing and development purposes.

First, uncomment line 13 in `_config.yaml`. Then run:

```
docker run -it --rm -v "$PWD":/usr/src/app -p "4000:4000" jataware/darpa-askem-docs
```