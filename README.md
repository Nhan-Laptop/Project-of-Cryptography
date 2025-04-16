# Elliptic-curve Cryptography
 Student: 
 - Nguyen Trong Nhan - 24521236
## Contents
- [Introduction]()
- [Elliptic Curves and Cryptography]()
  1. [Elliptic Curves]()
  3. [Elliptic Curves over Finite Fields]()
  4. [The Elliptic Curve Discrete Logarithm Problem]()
     - [The Double-and-Add Algorithm]()
     - [The Hard Problem of ECC]()
  5. [Elliptic Curves Cryptography]()
     - [The Basic Setup]() 
     - [Diffie-Hellman Key Exchange](https://) 
     - [ElGamal Public Key Encryption ](https://)
     - [ElGamal Digital Signatures](https://) 
     -    [ The Digital Signature Algorithm ](https://)
- [ECC Attacks]()
  1. [ECDH Attacks]() 
        - [The Order Of The Generator Is Too Small]()
        - [The Order Of The Generator Is A Smooth Number]()
        - [The Order Of The Generator Is Almost A Smooth Number, And The Private Key Is Small]()
        - [Not Verifying That A Point Is On The Curve]()
        - [The Curve Is Singular]()
        - [The Curve Is Supersingular]()
        - [The Curve Is Anomalous]()
  2. [ECDSA Attacks]()
        - [Not Hashing The Message Before Signing It](https://)
        - [Reusing The Same Value Of k In Different Signatures](https://)
        - [Generating k Values Insecurely](https://)
        - [Not Verifying The Generator Is Valid](https://)
   
 
## Introduction 
This article is devoted to introducing elliptic curves. Some of the more modern public key systems make use of elliptic curves since they can offer improved efficiency and bandwidth.\
Elliptic curves are applicable for key agreement, digital signature, pseudo-random generators, and etc.\
Elliptic Curve Cryptography (ECC) is a form of public-key cryptography that relies on the algebraic properties of elliptic curves defined over finite fields. Compared to traditional systems like RSA and ElGamal, which are based on modular exponentiation in Galois fields, ECC achieves the same level of security using significantly smaller key sizes.
## Elliptic Curves and Cryptography 
### 1. Elliptic Curves.
An Elliptic Curves $E$ is a set of is the graph of the form

$$
 Y^2 = X^3 + A.X + B
$$

where A and B are constants. This will be referred to as the Weierstrass equation of an elliptic curve. We will denote that A,B,x are belong to a set. Usually, they will be taken to be a set of elements of a field, for instance, the real number $\mathbb{R}$, the complex bumbers $\mathbb{C}$, the rational number $\mathbb{Q}$, one of the finite fields $F_p \ (=Z_p)$ for a prime p, or one of the finite fields $F_q$, with $q=p^k\ | \ k \in [1,\infty]$ .
In this article, let's assume that: $K$ be any field, the set of points in $E$ if defined over $K$.

