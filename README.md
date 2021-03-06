# wordlock
---text encryption/cipher with QT GUI---
*Wordlock project*
Brief introduction:
Wordlock project aims at encrypting/ciphering plain text using pseudo-random shuffling and pseudo-random letter injection. The random letter injection is a novel theory that we have developed to make the unauthorized decryption/deciphering much harder against brute forcing. 
The idea and the code were developed by Mehrdad S. Beni as a fun weekend project. 

How to:
Wordlock has a GUI developing using QT5 libraries and the program was written purely in C++ programming language. Initially, wordlock was developed on MacOS and GNU/Linux platforms. Later, we have further developed the program for Microsoft windows platforms and tested it on Windows 7 and Windows 11 machines. 
Run “wordlockQT.exe”
Enter the plain text you would like to encrypt/cipher at “enter text” dialog box.
Make sure no spaces between each word, spaces make brute forcing easier, you can separate your words by “-”.
At the right had side of the GUI, you can see “cklog1”, “cklog2”, “ckchar1”and “ckchar2”. These variables will be used for our newly developed algorithm of word injection module.
For simplicity, you can set “cklog1” and “cklog2” to any integer number between 0 to 10. The GUI is automatically set to some values for ease of use, mainly if you are lazy to set these! 
For the other 2 inputs, (i.e., ckchar1 and ckchar2), you can set any single character from your keyboard. The GUI is automatically set to some values for ease of use, mainly if you are lazy to set these!
Click on “Cipher” and in the output dialog you can see a red highlight, that is the cipher text without random letter injection module. The public cipher text that you can safely send to anyone without being easily understood will be stored in “wordlock.dat”. 
This file is in the same folder where you have executed the wordlock program. 
“wordlock.dat” is the encrypted plain text, please check and see if you can make any sense of the cipher text in this file, it would be hard!
In the same program folder, “key.dat” would be generated and that is your private key. Upon having this key, users can decrypt/decipher your secret message! 
You can simply click on “Decipher” to see the recovered message. This can also be seen in “revealdem.dat” file in the program folder. 
If you wish to lock other messages, you need to close the program and run again.
Every time you run, the random sequence will change, which means if you are not happy with the level of randomness, you can re-run the program to generate other sets of random sequences. 
Secret message from someone:
If you have received a secret message from someone that used our program, you can simply copy the encrypted/cipher text into wordlock.dat file and replace the key.dat file with the key.dat sent to you privately. Then simply click on “Decipher”.
