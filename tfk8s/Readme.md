
# translate kubernetes manifest file to terraform with tfk8s

## from https://github.com/jrhouston/tfk8s

for those of us that doesn't have golang installed, or have no idea of what golang is at all.

run command example:

```bash
docker run -it --rm -v $PWD/ns.yml:/ns.yml sinawic/tfk8s -f /ns.yml
```

or you can simply copy `tfk8s` executable file from inside the container to your linux system.

in a terminal hit:

```bash
docker run --rm -it --entrypoint /bin/bash --name tfk8s sinawic/tfk8s
```

then in another terminal:

```bash
docker cp tfk8s:/go/bin/tfk8s $PWD/tfk8s
sudo cp tfk8s /usr/bin/tfk8s
tfk8s --help
```

also to build the image yourself which will grab the latest `tfk8s` version, hit:

```bash
docker build -t sinawic/tfk8s .
```

> WITH ❤ BY SINAWIC
