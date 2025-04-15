# encryption-and-decryption-program
https://shanthosh-pro.github.io/encryption-and-decryption-program/

# 🔐 Simple End-to-End Encryption in Python

This is a simple Python project that demonstrates how end-to-end encryption works, similar to how secure messaging apps (like WhatsApp) protect your messages.

The app uses a combination of **RSA** (for key exchange) and **AES (Fernet)** (for message encryption), allowing two parties to send and receive encrypted messages securely.

---

## 💡 How It Works

- Each user (e.g., Alice and Bob) generates a public-private RSA key pair.
- When Alice wants to send a message to Bob:
  - She generates a random symmetric key (Fernet).
  - Encrypts the actual message with the symmetric key.
  - Encrypts the symmetric key using Bob's public RSA key.
- Bob uses his private key to decrypt the symmetric key, and then decrypts the message.

This ensures that **only Bob can read the message**, even if someone intercepts the communication.

---

## 🛠️ Requirements

Make sure you have Python 3.7+ installed.

Install the required package:

```bash
pip install cryptography
 
