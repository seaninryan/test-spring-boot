To build it from directory `/src/main/docker` (uses symlink)
```bash
docker build -t test-spring-boot
```

To run it
```bash
docker run -p 8080:8080 -d test-spring-boot
```

To look at the log output
```bash
docker logs <container-id>
```

To find the ip address it's running on (mac only)
```bash
docker-machine ls
```