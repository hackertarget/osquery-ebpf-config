# osquery ebpf configuartion example

An example configuration for running osquery on a Linux Server using the eBPF event system. 

## What is eBPF?

eBPF is a new way to collect event data within osquery. Rather than using the Linux audit subsystem it is based on collecting event data from the kernel using newer functionality. Requires kernel 4.18+.

These configuration files are based on the excellent configuration for osquery from [Palantir](https://github.com/palantir/osquery-configuration/tree/master/Classic/Servers/Linux). In addition to the published configurations they also provided a detailed [blog post](https://blog.palantir.com/osquery-across-the-enterprise-3c3c9d13ec55).

Modifications to the files include the osquery table changes for the process and socket event tables. In addition as tables have slightly different fields these have also been slightly tweaked. 

The idea is to use this configuration as a basis for doing testing of osquery prior to production deployment. 

## Further Information

We have a full [osquery tutorial](https://hackertarget.com/osquery-linux-tutorial/) over on our blog that includes additional information.




