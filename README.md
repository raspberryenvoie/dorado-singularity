# dorado-singularity
A singularity container for dorado.

## I. Usage

### A. Build

```bash
wget -qO- https://raw.githubusercontent.com/raspberryenvoie/dorado-singularity/refs/heads/main/build.sh | bash
```
This should take ~ 5 min.

### B. Run dorado

```bash
singularity run --nv dorado.sif dorado <parameters> # `--nv` allows the use of GPU
```

> Example: `singularity run --nv dorado.sif sh -c "dorado basecaller hac file.pod5 > file.bam"`

## II. Container implementation

The official [dorado docker container](https://hub.docker.com/r/nanoporetech/dorado) is used as a reference to build the container.
