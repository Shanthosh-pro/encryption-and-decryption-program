# 🔐 End-to-End Encryption Demo

Welcome to the **End-to-End Encryption Demo**! This is a fun, hands-on project where you can try out encryption in real-time using **RSA** (for key exchange) and **Fernet** (for encrypting messages). It’s a great way to see how secure communication works under the hood.

### 🌐 Try It Live

Want to see it in action? Check out the demo site here:

👉 [Test the Encryption Demo](https://shanthosh-pro.github.io/encryption-and-decryption-program/)

Feel free to play around, encrypt some messages, and see how it all works!

### 🔍 How It Works

Here’s a quick rundown of how the encryption process flows in this demo:

1. **RSA Key Pairs**: 
   - You (or anyone) generate a pair of RSA keys—**public** and **private**. The public key is shared with anyone you want to communicate with, while the private key stays secret.
   
2. **Encrypting a Message**:
   - When you send a message, you first encrypt it using a **symmetric key** (which is super fast and secure).
   - But how do you send that key? You **encrypt the symmetric key** with the recipient's **public RSA key**.
   
3. **Decrypting a Message**:
   - The recipient uses their **private RSA key** to decrypt the symmetric key.
   - Then, they use that key to decrypt the message, and voilà—your secret message is safely readable again!

### 🔧 Tech Stack

Here’s the tech behind it:

- **HTML/CSS**: The structure and styling to make it look nice.
- **JavaScript**: For the encryption and decryption magic. We’re using **Web Crypto API** for RSA encryption and **Fernet** for the symmetric encryption.
- **RSA-OAEP**: The asymmetric encryption for securely sending the symmetric key.
- **Fernet**: AES-based symmetric encryption for the actual message.

### 📝 How to Use

1. **Generate Keys**: 
   - Hit the **Generate Key Pair** button, and you’ll get a public and private key pair. Share the public key with anyone you want to send secure messages to.
   
2. **Encrypt a Message**: 
   - To send a secret message, paste the recipient’s public key into the box, type your message, and click **Encrypt**.
   
3. **Decrypt a Message**: 
   - If you’ve received a secret message, paste the encrypted message and your private key into the decryption box, then click **Decrypt** to read it!

### 🛠️ Running It Locally

1. Clone this repo:
   
   ```bash
   git clone https://github.com/yourusername/e2e-encryption-demo.git
   ```

2. Open `index.html` in your browser, and you’re ready to test the encryption demo locally!

---

### ⚠️ Security Note

Just a heads up—this demo is for educational purposes only. It shows how encryption works in a simple way, but it's **not** secure enough for real-world, production use. Use this for learning, not for storing sensitive information!

---

### 🤝 Contributing

Feel free to fork the project, open issues, or contribute improvements! If you find a bug or have a cool feature idea, let me know.

---

### 🙋‍♂️ Let’s Connect

If you have any questions, or if you just want to chat about encryption, feel free to reach out or open an issue. Let’s keep learning together!

---

