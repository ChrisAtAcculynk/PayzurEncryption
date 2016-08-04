#Demos
##Demo 1
Demo 1 uses the [`JSEncrypt`](https://github.com/travist/jsencrypt) and [`JQuery`](https://jquery.com/) libraries. It takes a user-entered plaintext message and a PEM-encoded RSA public key and returns the message after encrypting it using the key.

####When the encrypt button is pressed:
1. A new `JSEncrypt` object is created [#](https://github.com/ChrisAtAcculynk/PayzurEncryption/blob/master/demos/demo1.html#L17)
2. Sets the public key of the `JSEncrypt` to the user's input [#](https://github.com/ChrisAtAcculynk/PayzurEncryption/blob/master/demos/demo1.html#L18)
3. Encrypts the given text using `JSEncrypt`'s `encrypt()` function [#](https://github.com/ChrisAtAcculynk/PayzurEncryption/blob/master/demos/demo1.html#L20)
4. Returns the encrypted message [#](https://github.com/ChrisAtAcculynk/PayzurEncryption/blob/master/demos/demo1.html#L21)

![Gif of demo1 in action](http://i.imgur.com/aW8Ry3S.gif)

##Demo 1\.2
Demo 1\.2 also uses [`JQuery`](https://jquery.com/), as well as a slightly modified version of `JSEncrypt`. This demo requires a hardcoded public key, and therefore will not work as-is.

####Setup
To hide the key from the viewer, we need to hardcode it into our `JSEncrypt` file. For the sake of preserving the integrity of the original files, I've created a new file called [jsencrypt-hardcode.js](https://github.com/ChrisAtAcculynk/PayzurEncryption/blob/master/lib) in the lib directory. The key needs to be defined on [line 4240](https://github.com/ChrisAtAcculynk/PayzurEncryption/blob/master/lib/jsencrypt-hardcode.js#L4240).

Once that is done it should work just like Demo 1, but instead of using a user defined key it will use the hardcoded key.

![Gif of demo1.2 in action](http://i.imgur.com/Rs0reKB.gif)

_Note that javascript does not support multiline strings so you will either need to remove the newlines from your key or add in escape characters:_

`var str = "Hello\

there\

friend!";`

or

`var str = "Hello\nthere\nfriend!";`