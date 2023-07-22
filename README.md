# `tracert` Extended

Windows `tracert` with extended geo-location and ISP info. E.g.,

~~~
  1    48 ms     4 ms    10 ms  192.168.2.2     LAN
  2    27 ms     6 ms     6 ms  192.168.71.1    LAN
  3    21 ms   146 ms    26 ms  100.86.52.1     LAN
  4    24 ms     6 ms     9 ms  61.152.53.114   CN, Shanghai, China Telecom (Group)
  5     *        *        *     Timeout
  6     *        *        *     Timeout
  7    29 ms    24 ms    12 ms  202.97.94.237   CN, Shanghai, CHINANET-BACKBONE
  8     *        6 ms     *     202.97.50.193   CN, Shanghai, CHINANET-BACKBONE
  9    79 ms    73 ms    74 ms  202.97.93.146   SG, Singapore, CHINANET-BACKBONE
~~~

## Usage

~~~
tracertex.py -dst DST [-hop HOP] [-ipv {4,6}]

options:
  -dst DST    Target IP/hostname
  -hop HOP    Max number of hops to search for target (default 32)
  -ipv {4,6}  Force using IPv4/v6
~~~