# Caesar-Cipher-Encryptor-and-Decryptor

This is a simple Python program that performs encryption and decryption of text using a basic Caesar Cipher algorithm. It allows the user to input a message, specify a key (shift value), and generate an encrypted or decrypted version of the message.

#Features

	•	Encrypt Message: Convert a plaintext message into an encrypted format.
	•	Decrypt Message: Revert an encrypted message back to its original plaintext form.
	•	Handles Both Cases: The program works with both uppercase and lowercase letters. Non-alphabetic characters remain unchanged.
How It Works

	1.	Encryption: Each letter in the message is shifted by the value of the key within the range of the English alphabet.
	2.	Decryption: The reverse of the encryption process, shifting each letter back by the key value.

The Caesar Cipher logic works as follows:
	•	For lowercase letters: ((ord(char) - ord('a') + key) % 26 + ord('a'))
	•	For uppercase letters: ((ord(char) - ord('A') + key) % 26 + ord('A'))

Code Explanation

Functions

	1.	encrypt(message, key)
	•	Takes a plaintext message and a key as input.
	•	Encrypts alphabetic characters by shifting them using the Caesar Cipher method.
	2.	decrypt(encrypted_message, key)
	•	Takes an encrypted message and the same key as input.
	•	Reverses the encryption process to return the original plaintext message.
	3.	main()
	•	Provides a user interface for the program.
	•	Collects input for the message and key, displays the encrypted and decrypted messages.
