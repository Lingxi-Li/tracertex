# `tracert` Extended

Windows `tracert` with extended country and ISP info. E.g.,

~~~
  1     2 ms     2 ms     2 ms  192.168.2.2     LAN
  2     7 ms     6 ms     5 ms  192.168.71.1    LAN
  3     8 ms     5 ms     8 ms  100.86.52.1     LAN
  4     *        *        *     Timeout
  5     *        *        *     Timeout
  6     7 ms     5 ms     7 ms  101.95.120.122  CN: China Telecom (Group)
  7     *        *        *     Timeout
  8     *        *        *     Timeout
  9     *        *       66 ms  202.97.93.158   SG: CHINANET-BACKBONE
~~~

~~~
usage: tracertex.py -dst DST

options:
  -dst DST    Target IP/hostname
~~~