### Description

A simple image encryption tool using pixel manipulation. You can perform operations like swapping pixel values or applying a basic mathematical operation to each pixel. Allow users to encrypt and decrypt images

### Usage:

  Encrypt an image:
      **python  image_encryption_tool.py  encrypt  input_image.jpg  123  encrypted_image.jpg**

  Decrypt an image:
      **python  image_encryption_tool.py  decrypt  encrypted_image.jpg  123  decrypted_image.jpg**

"123" is an example value for the **encryption/decryption key**. It is a numeric value used to manipulate pixel values during the encryption and decryption processes.

- **Encryption**: Each pixel's value is increased by the key (`+ key`) and wrapped within the valid range of 0–255 using the modulo operation (`% 256`).
- **Decryption**: Each pixel's value is decreased by the same key (`key`) and similarly wrapped within 0–255.

The range **0–255** represents the possible values for each color channel (red, green, blue) in an image's pixel in the **8-bit color depth** format.
