# Start

```bash
docker run -it -d --name eiplatform \
  -v $(pwd)/logs:/opt/pilotfish/logs \
  -v $(pwd)/license:/opt/pilotfish/license \
  -v $(pwd)/eip-root:/opt/pilotfish/eip-root \
  -v $(pwd)/config:/opt/pilotfish/config \
  -p 8080:8080 \
  pilotfishtechnology/eiplatform
```

# Stop

```bash
docker stop eiplatform
```

# View Logs

```bash
docker logs -f eiplatform
```

# Upgrade

```bash
docker stop eiplatform
docker rm eiplatform
docker pull pilotfishtechnology/eiplatform
docker run -it -d --name eiplatform \
  -v $(pwd)/logs:/opt/pilotfish/logs \
  -v $(pwd)/license:/opt/pilotfish/license \
  -v $(pwd)/eip-root:/opt/pilotfish/eip-root \
  -v $(pwd)/config:/opt/pilotfish/config \
  -p 8080:8080 \
  pilotfishtechnology/eiplatform
```