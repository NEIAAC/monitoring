# Like CCTV, but for the server 📸🚨

- If using Loki with locally running processes you should also install Promtail, since we're only using Loki to for Docker container logs we don't need Promtail.
- Install the Loki Docker driver plugin to make docker automatically send container logs to Loki:

  ```shell
  docker plugin install grafana/loki-docker-driver:2.9.2 --alias loki --grant-all-permissions
  docker plugin ls
  ```

- Change the default logging driver to the newly installed plugin:

  ```shell
  nano /etc/docker/daemon.json
  ```

  - Edit the default Docker logs config, you must manually change the `{REPLACE}` to the `LOKI_PORT` from the `.env` file:

    ```json
    {
        "debug" : true,
        "log-driver": "loki",
        "log-opts": {
            "loki-url": "http://localhost:{REPLACE}/loki/api/v1/push",
            "loki-batch-size": "400",
            "loki-retries": "3",
            "loki-max-backoff": "800ms",
            "loki-timeout": "3s"
        }
    }
    ```

- Restart Docker to apply the changes, note that all containers not set to restart automatically will be stopped:

  ```shell
  systemctl restart docker
  ```

- If you ever need to update the Docker driver plugin do it like so:

  ```shell
  docker plugin disable loki --force
  docker plugin upgrade loki grafana/loki-docker-driver:new-version --grant-all-permissions
  docker plugin enable loki
  systemctl restart docker
  ```

- Start the docker compose file:

  ```shell
  docker compose up --force-recreate
  ```

- To update any of the services simply bump the version number in the `image` field and run the `docker compose up --force-recreate` command again, but beware of breaking changes! You should look at the update notes of each service to see if there are any migration steps required when upgrading.
