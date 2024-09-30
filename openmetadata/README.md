# OpenMetadata

## Getting Started
```sh
# Copy sample demo data.
cp -r ../demo_data/* spark-example/data

# Set UID which will be passed to the jupyter container so it can write to the host volume.
export UID=$(id -u)

# Start containers.
docker compose -f docker/compose.yaml up
```

We can now access OpenMetadata at http://localhost:8585 with the following credentials:
- Username: admin@open-metadata.org
- Password: admin

OpenMetadata ships with an Airflow container to run the ingestion workflows. We can access Airflow at http://localhost:8081. Use the following credentials to log in to Airflow.
- Username: admin
- Password: admin

and Jupyter Notebook on the following URL: 
- Jupyter Lab: http://localhost:8888/lab/tree/notebooks/openmetadata_demo.ipynb?token=easy

## Clean up

```sh
docker compose -f docker/compose.yaml down --volumes
```

## Refs
1. https://docs.open-metadata.org/v1.5.x/quick-start/local-docker-deployment
