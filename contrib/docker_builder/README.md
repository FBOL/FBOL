# Dockerfile for building FBOL binaries.

Now, you can build your own FBOL files on all systems with docker and do it easy without installing depends on your system.

## How:

### Build docker image

```
sudo docker build .
```

### Run docker container

Builder will return HASH of image
Example:
Successfully built 9bbff825d50f

```
sudo docker run -it -v ~/path/to/FBOL/folder:/FBOL 9bbff825d50f
```

If your system uses SELINUX you may use --privileged=true key

```
sudo docker run --privileged=true -it -v ~/development/FBOL:/FBOL 9bbff825d50f
```

See FBOL-qt file in used FBOL folder and FBOLd file in src subfolder.