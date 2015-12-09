# gitlab-docker-runner
GitLab docker runner

This is a gitlab runner include docker binary.

how to use this image

```bash
docker run -d \
    --name gitlab-runner \
    --restart always \
    -v /var/run/docker.sock:/var/run/docker.sock \
    -v /srv/gitlab-runner/config:/etc/gitlab-runner \
    djx339/gitlab-docker-runner
```

```bash
docker exec -it gitlab-runner gitlab-runner register

```

executor choice **shell**
