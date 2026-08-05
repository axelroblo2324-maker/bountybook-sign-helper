# BountyBook sign helper

Static, dependency-free helper for signing a single BountyBook nonce with an EVM wallet.

- It accepts the expected address and exact message through URL parameters.
- It uses only `eth_requestAccounts` and `personal_sign`.
- It never asks for a private key, recovery phrase, token approval, or transaction.
- It has no analytics, network requests, or third-party scripts.

Before use, generate a fresh nonce from the official BountyBook API and encode it in the URL. Do not reuse an old nonce.
