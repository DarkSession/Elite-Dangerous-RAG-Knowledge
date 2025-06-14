## Cmdr Backflaps &#8211; A Guide to Analysing Octal Messages

Published: 05 Jul 2017 on Canonn (https://canonn.science/media/cmdr-backflaps-a-guide-to-analysing-octal-messages/)

Content: **Cmdr Backflaps** (also known as Kal/Kalearne) presents a useful guide to **analysing octal messages** from the **Unknown Link**. This is the method used for locating additional **Unknown Sites**, but is also relevant to analysing **Unknown Probe** messages.

Cmdr **Redden Alt Mer** then gives details on how to **translate** the transcribed audio into a set of distances from **Merope** that then lets you identify the final location:

```text
The signal received from the UL can be translated to binary, considering high
tones as 0s and low tones as 1s. Using message #1 in our current example, this:
hhl hlh hll / lll llh lhh
lll / lll llh lhh
hll lhh lhl / hll lll hlh

becomes this:
001 010 011 / 111 110 100
111 / 111 110 100
011 100 101 / 011 111 010

Once we have the binary, each couple represent two operands, a dividend and a
divisor. To pass from this binary representation to the actual numbers, we
need to first translate each octet (e.g., 001) into a single digit:
001 -> 1
010 -> 2
011 -> 3
...

Doing so for the first set of operands, for example, will give us the following:
123 / 764

From our previous studies on the UP signal, and from observation (all the
digits are always in the [0-7] range), we can assume that this must be
interpreted as octal numbers (which are normally represented with a prefix 0 to
distinguish them from decimal numbers). Converting them to decimal, will give
us:
83 / 500

All that's left to do is to apply the division to all of the three and get
a measure of the distance, respectively from Merope, the system where the
message was collected, and Col 70 Sector FY-N c21-3, expressed in ThargMeters
(THm), i.e., the distance between Merope and Col 70 Sector FY-N c21-3, roughly
871.02Ly.

Applying the steps above to message #1 of our current example, we get:
0123/0764 -> 83/500 = 0.1660THm -> 144.5883Ly
07/0764 -> 7/500 = 0.0140THm -> 12.1942Ly
0345/0372 -> 229/250 = 0.9160THm -> 797.8487Ly

These three distances will allow us to trilaterate the next system pointed by this message.
```

Note that translating each binary triplet singularly to octal and then to decimal is optional. By directly merging each distinct set of binary triplets in a single binary number and then translating it to decimal will yield the same result. Applying it to the example above 001 010 011 ->  001010011 -> 83