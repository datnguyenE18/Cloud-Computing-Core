# **Cloud Encryption**




- Encryption plays a key role, and is often referred to as the last line of defense, in a layered security model
 
- It not only encrypts data, but also provides robust data access control, key management, and certificate management
![image](https://user-images.githubusercontent.com/43572616/180048999-8a028d7b-b387-4065-99f7-26383c5294c5.png)


- Encryption is defined as scrambling data in a way that makes it illegible. There are two parts to an encryption system—the encryption algorithm and the decryption key
![image](https://user-images.githubusercontent.com/43572616/180049047-050624bf-4e54-4791-a7e5-9efc5da457b1.png)
![image](https://user-images.githubusercontent.com/43572616/180049077-d814519c-4cf8-4d81-98fe-ece87de45dbf.png)



- Data is encrypted upon receipt, and encryption keys are passed to the customers to decrypt data when needed
 
- Data needs protection in three states
  - at rest - protects data while it is physically stored in a database or the storage layer 
  - in transit - protects data while it is transmitted from one location to another (encrypting the data before transmission, authenticating endpoints, and decrypting and verifying data on arrival. Secure Sockets Layer (or SSL) and Transport Layer Security (TLS) are commonly used protocols for encryption in transit)
  - in use - protects data when it is in use in memory for computations (It allows computations to be performed on encrypted text without needing to decrypt the data)
 
- Cloud storage encryption could be server-side or client-side
 
- Some of the best practices for encryption key management include: 
  - Storing encryption keys separately from the encrypted data. 
  - Taking key backups offsite and auditing them regularly. 
  - Refreshing the keys periodically. 
  - Implementing multi-factor authentication for both the master and recovery keys
