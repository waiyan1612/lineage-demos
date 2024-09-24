# Spline

## Getting Started
```sh
# Copy sample demo data.
cp -r ../demo_data/ spark-example/data

# Set UID which will be passed to the jupyter container so it can write to the host volume.
export UID=$(id -u)

# Start containers.
docker compose -f docker/compose.yaml up
```

You can access Spline services on the following URLs:
- Spline Web UI: http://localhost:9090
- Spline Server: http://localhost:8080

and Jupyter Notebook on the following URL: 
- Jupyter Lab: http://localhost:8888/lab/tree/notebooks/spline_demo.ipynb?token=easy

## Refs
1. https://github.com/AbsaOSS/spline-getting-started
2. https://github.com/AbsaOSS/spline-spark-agent
