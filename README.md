# Data-Storage-on-Cloud-using-Split-Merge-and-Hybrid-Cryptographic-Techniques

Overview

This project focuses on designing and implementing a secure cloud-based text file storage solution that leverages advanced cryptographic algorithms and split-merge techniques to enhance data security and integrity. The primary goal is to ensure the confidentiality, integrity, and availability of data stored in the cloud.

Objectives

- To design a secure storage solution for text files on the cloud.
- To implement hybrid cryptographic techniques, including AES, DES, and RSA, for encrypting and decrypting data.
- To optimize encryption and decryption processes for efficiency.
- To employ split-merge techniques to further enhance data security and integrity.

Cryptographic Techniques

AES (Advanced Encryption Standard)
AES is a symmetric encryption algorithm widely used for its security and efficiency. In this project, AES is used for encrypting data in a way that ensures confidentiality and fast processing.

DES (Data Encryption Standard)
DES is another symmetric encryption algorithm used in this project for its simplicity and historical significance. Although considered less secure than AES, it is included to demonstrate multiple encryption methods.

RSA (Rivest-Shamir-Adleman)
RSA is an asymmetric encryption algorithm used for securely exchanging keys. This project uses RSA to securely share encryption keys between the client and the server.

Split-Merge Technique

The split-merge technique involves splitting the data into smaller chunks before encryption and storing them separately. This method provides several benefits:
- Enhanced Security**: Even if an attacker gains access to a part of the data, they cannot decrypt it without all the pieces.
- Data Integrity**: Splitting and merging ensure that the data remains intact and unaltered.
- Efficiency**: Smaller chunks of data can be processed faster and more efficiently.

Implementation Details

1. Data Splitting
The text file is divided into smaller chunks. This step is crucial for managing large files and ensuring efficient processing.

2. Encryption
Each chunk is encrypted using a combination of AES, DES, and RSA. AES and DES are used for the actual data encryption, while RSA is used for securely transmitting the encryption keys.

3. Storage
The encrypted chunks are stored on the cloud. Each chunk is stored in a different location to maximize security.

4. Key Management
Keys are managed using RSA, ensuring that encryption keys are securely shared between the client and the server. This prevents unauthorized access to the encryption keys.

5. Data Merging
When a user needs to access the stored data, the chunks are retrieved, decrypted, and merged to form the original text file.

Technologies Used

- Programming Languages**: Python for the main implementation.
- Cryptographic Libraries**: PyCrypto, Cryptography for implementing AES, DES, and RSA.
- Cloud Storage Services**: AWS S3, Google Cloud Storage for storing encrypted chunks.
- Other Tools**: Docker for containerizing the application, ensuring consistent deployment environments.

Advantages

- High Security**: Combines multiple encryption algorithms and split-merge techniques to provide robust security.
- Efficiency**: Optimized encryption and decryption processes ensure fast performance.
- Scalability**: Designed to handle large files and scale with cloud storage solutions.
- Data Integrity**: Ensures data integrity through splitting and secure key management.

Future Work

- Enhanced Key Management**: Implementing more sophisticated key management solutions like AWS KMS or Azure Key Vault.
- User Interface**: Developing a user-friendly interface for easier interaction with the storage system.
- Performance Optimization**: Further optimizing the encryption and decryption processes for even better performance.

Conclusion

This project demonstrates a comprehensive approach to securing data storage on the cloud using hybrid cryptographic techniques and innovative split-merge methods. It addresses key concerns in cloud security and provides a scalable, efficient, and secure solution for storing sensitive data.

