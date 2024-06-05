# IPv6 Addressing

An IPv6 address consists of 32 hexadecimal digits, in 8 sections of 4 digits each, separated by colons. It looks something like this: 1234:5678:90ab:cdef:1234:5678:90ab:cdef

IPv6 addresses have several shortcuts that allow them to be compressed into smaller strings following certain rules.
Shortening Rule

If there are any leading zeroes in a section, they may be left off. 0001:0001:0001:0001:0001:0001:0001:0001 could be written as 1:1:1:1:1:1:1:1.

Any number of address parts consisting of only zeroes may be compressed by using :: but this can only be done once in an IPv6 address to avoid ambiguity. 

 0000:0000:0000:0000:0000:0000:0000:0001 to ::1. 

Any time :: appears in an IPv6 address, the values between are all zeroes. An IP address such as fe80:1111:2222:0000:0000:0000:7777:8888, can be represented as fe80:1111:2222::7777:8888. 

However, fe80:1111:0000:0000:4444:0000:0000:8888 cannot be shortened using :: more than once. It would either be fe80:1111::4444:0:0:8888 or fe80:1111:0:0:4444::8888 but it cannot be fe80:1111::4444::8888 because there is no way to tell how many zeroes have been replaced by either :: operator.
