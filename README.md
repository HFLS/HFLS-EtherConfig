We find that chinahw.net server is located at HFLS. Through traceroute we identify that there are 4 steps:
```bash
 1  192.168.2.1 (192.168.2.1)  1.778 ms  3.555 ms  3.600 ms
 2  172.16.56.254 (172.16.56.254)  7.334 ms  7.337 ms  7.332 ms
 3  172.16.0.29 (172.16.0.29)  7.325 ms  7.318 ms  7.309 ms
 4  172.16.0.42 (172.16.0.42)  13.859 ms  13.832 ms  13.842 ms
```
And thus we can map the physical path the data transferred.
According to this table, 
```bash
 1  192.168.2.1 (192.168.2.1)  1.778 ms  3.555 ms  3.600 ms       // The router for each class 
 2  172.16.56.254 (172.16.56.254)  7.334 ms  7.337 ms  7.332 ms   // The router for #5 F3-4
 3  172.16.0.29 (172.16.0.29)  7.325 ms  7.318 ms  7.309 ms       // Unknown, might be the central router (but why not gateway?)
 4  172.16.0.42 (172.16.0.42)  13.859 ms  13.832 ms  13.842 ms    // Unknown. 
```

What else can be refered from those info?
