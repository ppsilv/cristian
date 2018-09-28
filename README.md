Cristian's algorithm implementation in C

Cristian's algorithm is a method for clock synchronisation which can be used in many fields of distributive computer science but is primarily used in low-latency intranets.

More information at:
http://en.wikipedia.org/wiki/Cristian%27s_algorithm

An example is implemented in C language using Knoppix GNU/Linux as operating system. It is based on TCP/IP. TCP/IP refers to two protocols that work together to deliver data: the Transmission Control Protocol (TCP) and the Internet Protocol (IP).

Cristian's algorithm example:
Send request at 5:08:15.100 (T0)
Receive response at 5:08:15.900 (T1)
Response contains 5:09:25.300 (Tserver)
Elapsed time is T1-T0
5:08:15.900 - 5:08:15.100 = 800 msec
Best guess: timestamp was generated 400 msec ago
Set time to Tserver + elapsed time
5:09:25.300 + 400 = 5:09.25.700
