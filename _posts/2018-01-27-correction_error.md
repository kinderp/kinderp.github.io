---
published: true
layout: post
categories:
   - binary_chats
---
This post should be the first about binary operations or more in general on low level discussions. This series might seem to you  just a lot heavy, but according to me it's the starting point to go far in our jourey.

The errors correction and detection has a unique milestone: a system that would be able to detect and correct
an error that has occurred in the encoding during a transmission must use more bits in the source code or alphabet.
In this way the enconding will have bit configurations that will be not used and an error will transform the
transmitted valid bit configuration in a not valid one.

### Fondamental definition

**Hamming distance** from two possibile binary configurations is the number of different bit between the two one

In practical to calculate the hamming distance it's sufficient apply an xor operation to the two binary configurations and then counting the number of ones in the result.

**Mininal distance** of a code is the minimal hamming distance between two whichever binary configurations of a code.

**Redundace code** is a code where the number of binary configurations are more than the encoded symbols  


