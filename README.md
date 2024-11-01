# README

## Description 

Container to mount a TrueCrypt file using version 7.1a. 

## How to Build

If you are in a M1 mac, you need `--platform=linux/x86_64`
```sh
docker build --platform=linux/x86_64 --tag=truecrypt:7.1a .
```

## Hot to run
```sh
docker run -it --platform=linux/x86_64 \
  --rm --privileged \
  --name truecrypt \
  -v ./share:/share \
  truecrypt:7.1a \
  /bin/sh
```


## Links

1. Source: https://github.com/DrWhax/truecrypt-archive
2. Docker file inspiration: https://github.com/pmjohann/truecrypt
