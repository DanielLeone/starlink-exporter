A very thing wrapper around the great work of: https://github.com/sparky8512/starlink-grpc-tools

Changes:
* Including a submodule with my own fork of [starlink-grpc-tools](https://github.com/DanielLeone/starlink-grpc-tools), so that I can get my bleeding edge changes in (ususally just adding some metrics)
* A copy/paste of the Dockerfile with the entrypoint modified to run only the Prometheus exporter with all the metrics available (so that you don't have to craft the entrypoint command yourself)
* A GitHub Actions workflow to build and push the docker images automatically

Docker images:
https://hub.docker.com/repository/docker/danleone/starlink-exporter
