# OpenLineage

## Getting Started
```sh
# Copy sample demo data.
cp -r ../demo_data/* spark-example/data

# Set UID which will be passed to the jupyter container so it can write to the host volume.
export UID=$(id -u)

# Start containers.
docker compose -f docker/compose.yaml up --build
```
If you observe errors from the `api` container on MacOS, check out https://github.com/MarquezProject/marquez/issues/2886#issuecomment-2322995719.

Marquez is a reference implementation of OpenLineage specification. You can access Marquez on the following URLs:
- Marquez GraphQL UI: http://localhost:5002/graphql-playground
- Marquez Admin UI: http://localhost:5001
- Marquez Web UI: http://localhost:3000

and Jupyter Notebook on the following URL: 
- Jupyter Lab: http://localhost:8888/lab/tree/notebooks/openlineage_demo.ipynb?token=easy

## Refs
1. https://github.com/MarquezProject/marquez/blob/0.49.0/docker/up.sh
