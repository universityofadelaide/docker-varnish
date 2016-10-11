Brutally simple [Varnish](https://varnish-cache.org/) image based on [Alpine](https://alpinelinux.org/). Designed to be used for checking VCL files for defects using the follwing `docker run` command:

```bash
$ docker run -v $(pwd):/etc/varnish uofa/varnish varnishd -C -f /etc/varnish/default.vcl
```

To build manually:

```bash
$ docker build -t uofa/varnish .
```
