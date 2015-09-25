Source https://spring.io/guides/gs/spring-boot-docker/

To build it from directory `/src/main/docker` (uses symlink)
```bash
docker build -t test-spring-boot
```

To run it
```bash
docker run -p 8080:8080 -d test-spring-boot
```

To run it with a profile
```bash
docker run -p 8080:8080 -d -e "SPRING_PROFILES_ACTIVE=PRO" e52768fd064f
```

To look at the log output
```bash
docker logs <container-id>
```

To find the ip address it's running on (mac only)
```bash
docker-machine ls
```

Next - try docker building with maven
