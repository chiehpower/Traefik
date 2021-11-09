# test-Traefik

```
cd test3
docker-compose up -d
```

Then you can check here:

```
http://localhost:8080/api/rawdata
```

And also test it by this:

```
curl -H Host:whoami.docker.localhost http://127.0.0.1
```

Try to scale your services

```
docker-compose up -d --scale whoami=2
```

Test it again:

```
curl -H Host:whoami.docker.localhost http://127.0.0.1
```

You can see the Hostname of output changing:

```
Hostname: a656c8ddca6c
IP: 172.27.0.3
#...

Hostname: s458f154e1f1
IP: 172.27.0.4
```

 ### Reference

- [Quick-Start](https://doc.traefik.io/traefik/getting-started/quick-start/)