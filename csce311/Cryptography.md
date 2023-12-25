
### Symmetric Key Cryptography
There needs to be a known shared key that both parties know



### Public Key Cryptography

**One way function**
- A function that is easy to do but hard to revers

**One way trapdoor function**
- Reverse is easier with some special information

##### TLDR
With a message $\large m$, and keys $\large K_{B}^{-}\text{ and } K_{B}^{+}$, the public and private key respectively
$$\large K_{B}^{-}(K_{B}^{+}(m)) = m = K_{B}^{+}(K_{B}^{-}(m))$$
It is built around factoring massive numbers (thousand bit type shiii)



### Application

Use Public key stuff to initialize a symmetric key between endpoints (session key)