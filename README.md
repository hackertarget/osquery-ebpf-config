# osquery ebpf configuartion example

An example configuration for running osquery on a Linux Server. 

## What is eBPF?

eBPF is a new way to collect event data within osquery. Rather than using the Linux audit subsystem it is based on collecting event data from the kernel using newer functionality. Requires kernel 4.18+.

These configuration files are based on the excellent configuration for osquery from [https://github.com/palantir/osquery-configuration/tree/master/Classic/Servers/Linux](Palantir).

Modifications to the files include the osquery table changes for the process and socket event tables. In addition as tables have slightly different fields these have also been slightly tweaked. 

The idea is to use this as a basis for doing testing of osquery prior to production deployment. We have a full [https://hackertarget.com/osquery-linux-tutorial/](osquery Linux tutorial) over on our blog.




