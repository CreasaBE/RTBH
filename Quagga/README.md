# RTBH

Quagga config scripts

---

Quagga has a 'bug' that if 192.0.2.1/32 is nullrouted and then set as next-hop in a route-map it will not install the routes learned from BGP to be nullrouted.
That is why I assign it to the lo interface.

Thus letting Quagga install the routes to be nullrouted and just send them to lo, since the lo interface is internal and can handle quite a lot of traffic

***
