# varnish-top #

**varnish-top** is inspired by [memcache-top](http://code.google.com/p/memcache-top/), which was in turn inspired by top.

Simply, it is a tool that lets you monitor a few key stats from one or more varnish boxes in real-time, from the command line, in a top-like screen.  It's not the most sophisticated tool, but is handy for seeing a real-time view into how your box(es) are doing without needing to set up graphing, open up a browser, etc.

Similar to varnishstat, but runs across multiple boxes.



### Sample output: ###
```
varnish-top v0.1        (default port:  6082, color: on, refresh: 3 seconds)

INSTANCE                USAGE   HIT %   TIME    OBJs    EXPIR/s NUKED/s REQ/s
10.50.200.112:6082      48.2%   40.0%   1.8ms   9471    0.0     0.0     2
10.50.200.79:6082       88.6%   62.5%   1.5ms   9075    0.0     0.0     3
10.50.200.87:6082       12.0%   60.0%   1.5ms   5033    0.7     0.0     3
10.50.45.90:6082        97.5%   50.0%   1.6ms   12.7K   0.0     0.0     1

AVERAGE:                61.6%   53.1%   1.6ms   9144    0.2     0.0     2

TOTAL:          4.9GB/  8.0GB           6.4ms   35.7K   0.7     0.0     9
(ctrl-c to quit.)
```