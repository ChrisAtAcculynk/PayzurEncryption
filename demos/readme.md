#Demos
##Demo 1
Demo 1 uses the [`JSEncrypt`](https://github.com/travist/jsencrypt) and [`JQuery`](https://jquery.com/) libraries. It takes a user-entered plaintext message and a PEM-encoded RSA public key and returns the message after encrypting it using the key.

####When the encrypt button is pressed:
1. A new `JSEncrypt` object is created [#](https://github.com/ChrisAtAcculynk/PayzurEncryption/blob/master/demos/demo1.html#L17)
2. Sets the public key of the `JSEncrypt` to the user's input [#](https://github.com/ChrisAtAcculynk/PayzurEncryption/blob/master/demos/demo1.html#L18)
3. Encrypts the given text using `JSEncrypt`'s `encrypt()` function [#](https://github.com/ChrisAtAcculynk/PayzurEncryption/blob/master/demos/demo1.html#L20)
4. Returns the encrypted message [#](https://github.com/ChrisAtAcculynk/PayzurEncryption/blob/master/demos/demo1.html#L21)
