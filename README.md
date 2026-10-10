# Diffie-Hellman Key Exchange

This project provides a simple Python implementation of the Diffie-Hellman key exchange protocol and a simulation of a Man-in-the-Middle (MITM) attack.

**This implementation is intended for educational purposes only and should not be used to secure real-world communications.**

## Implementation Notes

- There is no actual network communication between Alice and Bob. The key exchange is simulated locally in Python.
- The `random` module uses the Mersenne Twister pseudorandom number generator. Although it is not cryptographically secure, it was used here to simulate random private exponent generation.
- A more realistic implementation could use two separate terminals for Alice and Bob, and a third terminal for Eve to demonstrate the MITM attack.
- No automated tests have been implemented yet.

## How to Run

```bash
dh.py
attacks.py
```

## References

- [RFC 7919 - Appendix A.2: ffdhe3072](https://www.rfc-editor.org/rfc/rfc7919.html#appendix-A.2) - Standardized 3072-bit finite-field Diffie-Hellman group, including the prime modulus \(p\), generator \(g=2\), and subgroup order \(q=(p-1)/2\).
