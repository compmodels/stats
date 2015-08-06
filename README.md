# compmodels/stats

Docker image for collecting JupyterHub statistics. Requires a token from JupyterHub, e.g.

    export token=$(jupyterhub token -f /path/to/jupyterhub_config.py jhamrick)
    docker run -e "JPY_ADMIN_TOKEN=$token" compmodels/stats --hub=http://[jupyterhub_ip]:8081