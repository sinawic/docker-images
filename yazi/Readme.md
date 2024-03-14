
# YAZI

## sinawic edition

this is a dockerization of https://github.com/sxyazi/yazi

### usage

`docker run -it --rm -v /filesystem:/filesystem sinawic/yazi /filesystem`

by default path will be `/`

### build yourself

after cloning the repo:

```bash
cd yazi
docker build -t sinawic/yazi .
```
