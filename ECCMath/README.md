# ECC - Elliptic Curves

Elliptic curves libraries are used to generate Private Keys, Public Keys and signatures for transactions.

Bitcoin and Ethereum both use secp256k1; the formula for the curve is `y^2 = x^3 + 7` over a finite field of `Fp`.

```
p = 2^256 - 2^32 - 2^9 - 2^8 - 2^7 - 2^6 - 2^4 - 1
```

The modulo prime number `p` is less than the finite field and just less than the maximum number of an unsigned 256 bit integer.

## Private Keys as Scalars

A private key is a scalar which is a member of `Fp`.

The private key is a highly random number from within the field `Fp` such that it is near impossible to guess or deduce.
