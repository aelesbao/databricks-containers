# Databricks Containers

This repository contains different containers that can be used in Databricks
clusters.

Additional information can be found in
[Customize Containers with Databricks Container Services](https://docs.databricks.com/clusters/custom-containers.html)
documentation.

## Images

### Data Engineering

The [data-engineering](./data-engineering/Dockerfile) image has support for:

- Scala Notebooks
- Java/Jar jobs
- Spark Submit Jobs
- DBFS FUSE (mounts DBFS to the local filesystem at `/dbfs`)
- SSH (with `ubuntu` user)
- %sh

> Since this image doesn't install Python, it requires at least the
**Databricks Runtime 6.0** to work with DBFS FUSE support.
