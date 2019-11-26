# ENNEoS
VERY ROUGH PROOF OF CONCEPT
Work in progress. 

Current status: Regularly being broken by me trying to stuff multiple shellcodes into neural networks. 

Evolutionary Neural Network Encoder of Shenanigans

This proof of concept program is to explore the use of
neuroevolution as a method for encoding shellcode.
The encoder uses genetic algorithms
to evolve a neural network that will output the desired
shellcode at runtime.

Lots of code borrowed from:
https://github.com/hoodoer/NEAT_Thesis

Drew Kirkpatrick
@hoodoer
drew.kirkpatrick@gmail.com




The encoder uses genetic algorithms to evolve neural networks that output the shell code on demand. 
The shellcode to be encoded into the neural networks is included in the "encodedOutput.h" file (not a great name). 

You can generate one of these header files from raw shellcode binaries using:
https://github.com/hoodoer/shellcodeEncryptor

Just skip the encryption options, it'll output a header file with your shellcode. 

This is most definitely a work in progress, but the initial demo works,
popping a meterpreter shell in Windows from shellcode output by the neural network


Good overview of the technique can be seen at my CackalackyCon talk:

https://youtu.be/nTb6SBGaLR8
