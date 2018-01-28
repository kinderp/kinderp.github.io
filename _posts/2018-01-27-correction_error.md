---
published: true
layout: post
categories:
   - binary_chats
---
This post should be the first about binary operations or more in general on low level discussions. This series might seem to you  just a lot heavy, but according to me it's the starting point to go far in our jourey.

As you already know a computer works just with binary numbers but it must be able to handle different types of informations like multimedia. Every type of different informations (videos, audios etc) must be encoded in a binary representations. This operation is called encoding.
More formally an **encoding** is a rule, an tranforming operation of a series of symbols into another one. The set of the symbols is called **alphabet**. Finally a **word** or **string**** is a sequence even repeated of an alphabet.

So to be more clear for example: i have two alphabets:

Alphabet | Set of symbols
------------ | -------------
Binary |{0,1}
Italian Alphabet |{a,b,c,...,z}

if i apply an ascii encoding i will able to represents an italian letter through a word of the binary alphabet just like this `a -{ascii}-> 01100001`

If the word of my representation are binary string my code is a **binary code**.

When we handle binary code it's important to define the lenght of the binary words or the number of bits used forming a word.
This number is important because is a constraint on the number of possible binary configurations (words) i can create and so
a restrinction on the number of symbols of the destination alphabet that the encoding is able to represent. 

The errors correction and detection has a unique milestone: a system that would be able to detect and correct
an error that has occurred in the encoding during a transmission must use more bits in the source code or alphabet.
In this way the enconding will have bit configurations that will be not used and an error will transform the
transmitted valid bit configuration in a not valid one.

### Fondamental definition

**Hamming distance** from two possibile binary configurations is the number of different bit between the two one

In practical to calculate the hamming distance it's sufficient apply an xor operation to the two binary configurations and then counting the number of ones in the result.

**Mininal distance** of a code is the minimal hamming distance between two whichever binary configurations of a code.

**Redundace code** is a code where the number of binary configurations are more than the encoded symbols  


