
# Hybrid AES and 3DES Encryption System

This project implements a hybrid encryption mechanism to securely encrypt and decrypt images. It combines AES-256 in CTR mode and 3DES to ensure robust and layered security. The dataset is encrypted and stored in a secure format, with easy decryption functionality for authorized access. This solution ensures data confidentiality and complies with stringent security requirements for sensitive data.

## About AES-256 (CTR Mode)
AES-256 (Advanced Encryption Standard) is a symmetric encryption algorithm recognized for its speed and strength. It uses a 256-bit key for encryption, making it resistant to brute-force attacks. The CTR (Counter) mode ensures high efficiency and eliminates the risk of data block duplication by using a unique counter value for each block of plaintext.

![Screenshot 2024-11-30 205909](https://github.com/user-attachments/assets/6f550249-0e0b-43b0-9d7b-b7855d420e8c)


## About 3DES (Triple DES)
3DES (Triple Data Encryption Standard) applies the DES algorithm three times in succession, strengthening its resistance to attacks. With a 24-byte (192-bit) key, 3DES provides enhanced encryption capabilities, making it a reliable component in multi-layered security systems.

![Screenshot 2024-11-30 205909](https://www.splunk.com/content/dam/splunk-blogs/images/en_us/2023/02/triple-des2.png)

## Project Flow

The encryption and decryption process follow a systematic flow:

**1) Dataset Loading:** Medical images are collected and prepared for processing.

**2) Key Generation:** AES and 3DES keys are generated and securely stored.


**3) Hybrid Encryption:**

- Images are encrypted with AES-256 in CTR mode.

- The AES-encrypted data is further encrypted using 3DES.


**4) Hybrid Decryption:**

- The encrypted data is decrypted using 3DES.

- The AES decryption process retrieves the original image.

**5) Output:** Encrypted and decrypted images are saved in respective directories.

![Frame 79](https://github.com/user-attachments/assets/10483ef2-847a-4eb6-9c2e-91813ff77d06)


## Why AES-256 CTR and 3DES?

**1) AES-256 CTR:**

- **Efficiency:** CTR mode allows parallel processing, making it faster for large datasets.

- **Security:** A 256-bit key ensures high resistance to brute-force attacks.

- **Uniqueness:** Nonce-based encryption eliminates data duplication risks.

**2) 3DES:**

- **Layered Security:** Acts as an additional encryption layer, enhancing data protection.

- **Proven Reliability:** Despite being older, 3DES remains robust against many attack vectors when used appropriately.

## How to Use

1) Clone the repository:

```bash
git clone https://github.com/Saisamarth21/Hybrid-AES-and-3DES-Encryption-System.git

cd Hybrid-AES-and-3DES-Encryption-System
```

2) Install the required libraries: 
```bash
pip install cryptography pycryptodome tqdm
```

3) Prepare your dataset and configure paths in the notebook.

4) Run the notebook sequentially to encrypt and decrypt the images.


