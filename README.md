rsWindows
==================
```PoSh

#rsHostsFile will add or remove all instances of a hostname from system Hosts file. Useful for setting custom resolvers on host.

rsHostsFile AddDemo
{
    Ensure = "Present"
    IPAddress = "127.0.0.1"
    HostName = "test1.local"
}

rsHostsFile RemoveDemo
{
    Ensure = "Absent"
    IPAddress = "127.0.0.1"
    HostName = "test2.local"
}
````