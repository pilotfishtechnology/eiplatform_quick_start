# Start

```bash
docker run -it -d --rm --name eiplatform \
  -v $(pwd)/logs:/opt/pilotfish/logs \
  -v $(pwd)/pflicense.key:/opt/pilotfish/license/pflicense.key \
  -v $(pwd)/eip-root:/opt/pilotfish/eip-root \
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
docker pull pilotfishtechnology/eiplatform
docker run -it -d --rm --name eiplatform \
  -v $(pwd)/logs:/opt/pilotfish/logs \
  -v $(pwd)/pflicense.key:/opt/pilotfish/license/pflicense.key \
  -v $(pwd)/eip-root:/opt/pilotfish/eip-root \
  -p 8080:8080 \
  pilotfishtechnology/eiplatform
```