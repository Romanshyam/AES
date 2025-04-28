# EX-8-ADVANCED-ENCRYPTION-STANDARD-DES-ALGORITHM
## Name: SHYAM KUMAR E
## Reg No: 212223230207
# Aim:
To use Advanced Encryption Standard (AES) Algorithm for a practical application like URL Encryption.

# ALGORITHM:
AES is based on a design principle known as a substitution–permutation.
AES does not use a Feistel network like DES, it uses variant of Rijndael.
It has a fixed block size of 128 bits, and a key size of 128, 192, or 256 bits.
AES operates on a 4 × 4 column-major order array of bytes, termed the state
# PROGRAM:
```
 #include <stdio.h>
 Preview Code Blame Raw
 Sign in
#include <string.h>
 void xor_encrypt_decrypt(char *input, char *key) {
 int input_len = strlen(input);
 int key_len = strlen(key);
 for (int i = 0; i < input_len; i++) {
 input[i] = input[i] ^ key[i % key_len];
 }
 }
 int main() {
 printf("\n\n\n\n      
char url[] = "WELCOME";
 char key[] = "secretkey"; 
printf("Original text: %s\n", url);
 xor_encrypt_decrypt(url, key);
 printf("Encrypted text: %s\n", url);
 return 0;
 }
 ***** ADVANCED-ENCRYPTION-STANDARD-DES-ALGORITHM *
 xor_encrypt_decrypt(url, key);
 printf("Decrypted text: %s\n", url)
```
# OUTPUT:
![image](https://github.com/user-attachments/assets/493173fb-1e6f-4b0b-9c96-f7231d3286b9)

# RESULT:
The experiment is successfully Executed.


