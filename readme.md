# Up/down swap patch applied 'iperf'

Usually `iperf` client sends data to iperf server, which is uplink test. Upon client' request, this package makes the server send data back to the client in the same connection, which is downlink test.

In a nutshell, this is a package for download speed test, using `iperf`. It works on tcp or udp layer, not http layer.

The base code is from [iperf-2.0.5](http://sourceforge.net/projects/iperf/), and [update patch](http://www.loria.fr/~lnussbau/) provided by Lucas Nussbaum was applied.

```bash
$ ./configure
$ make
$ ./src/iperf
```

**`NOTE`** This project was prepared for my another project, [iperf-stress](https://github.com/appkr/iperf). This acts as a sub-module of that project.