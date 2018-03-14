# ping_exporter
Prometheus exporter for ICMP echo requests using https://github.com/digineo/go-ping

This is a simple server that scrapes go-ping stats and exports them via HTTP for
Prometheus consumption. The go-ping library is build and maintained by Digineo GmbH.
For more information check the [source code][github].

[github]: https://github.com/digineo/go-ping

## Getting Started

To run the exporter via:

```bash
./ping_exporter [options] target1 target2 ...
```

Help on flags:

```bash
./ping_exporter --help
```

### Docker

https://hub.docker.com/r/czerwonk/ping_exporter

To run the ping_exporter as a Docker container, run:

```bash
docker run -p 9427:9427 --name ping_exporter czerwonk/ping_exporter
```


## Contribute

Simply fork and create a pull-request. We'll try to respond in a timely fashion.

## License

MIT License, Copyright (c) 2018
[Philip Berndroth][pberndro]
[Daniel Czerwonk][dan_nrw]
[pberndro]: https://twitter.com/pberndro
[dan_nrw]: https://twitter.com/dan_nrw
