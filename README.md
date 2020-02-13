# Jenkins Master Dockerize

## Setup Jenkins Server
  ```
    prahveen@geeklab$ docker compose up -d
  ```

## Get default admin password
  ```
    prahveen@geeklab$ docker exec -it {container_name} /bin/sh
    $ cat /var/jenkins_home/secrets/initialAdminPassword
  ```