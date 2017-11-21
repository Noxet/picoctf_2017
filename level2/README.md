# Cryptography

## SoRandom
Just reverse the algorithm.

The flag is
`FLAG:3b1fa718577cd90efb2fdf5832b6a849`

---

## LeakedHashes

---

## Weird RSA
Using the Chinese Remainder theorem, we can compute the private key and decrypt the message. Then we convert the number into the corresponding ascii values.

The flag is

`Theres_more_than_one_way_to_RSA`

---

# Reverse Engineering

## A Thing Called the Stack
The return address lies right above the saved stack frame (ebp). Then, we have 4 push instructions that pushes 4 bytes each. Next we have the sub instruction that moves the stack pointer 0xf8 bytes further. In total, the distance between the esp and the return address is 264.

The flag is

`0x108`

---

## Programmers Assemble
To get out of the loop, eax must be zero. each round, ebx is incremented by 5 (the value of ecx). In the _fin_ function, we need ebx to be 0x8f2f. Thus, we must have run the loop for a fifth, i.e. 7331 number of times. We must load eax with this value, in hex.

The flag is

`0x1ca3`

---

# Web Exploitation

## My First SQL
Just a simple SQL injection a la

`' OR '1'='1`

The flag is

`be_careful_what_you_let_people_ask_1b3db77df6b116a38db8ceb7c81cb14c`

---
