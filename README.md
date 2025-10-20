# portfolio

I would like to share some projects from my software portfolio

The projects included in this list give an introduction to socket programming, graphics, object-oriented programming, object-oriented design, modular design, GUIs, encryption, and many other topics in computer science

(I might also add, byte arithmetic, bit arithmetic, packets, etc)

I can organize my portfolio as a list of projects, and attach notes to each item in the list

You can find the list of projects below

1. [chat](https://github.com/ataylor89/chat)
    - This is an open-source chat server (kind of like an IRC server)
    - I was able to deploy it successfully to AWS cloud, and run it successfully on AWS cloud
    - It uses the RSA encryption algorithm to encrypt packets that are exchanged between client and server
    - It uses a custom protocol that is built ontop of the TCP protocol
    - It uses custom packets, and each custom packet is contained within the body of a larger TCP packet
    - It uses a file database (or a serial database) to store user accounts and user passwords
    - This project teaches us a lot about socket programming, packets, protocols, the TCP/IP stack, encryption, databases, etc
2. [Paint](https://github.com/ataylor89/Paint)
    - This is an open-source paint application (kind of like MS Paint on Microsoft Windows)
    - I think it serves as a very good introduction to graphics
    - It can serialize an image to file and deserialize a file to image
    - It uses a lot of math behind the scenes
    - It uses the Java Swing framework and draws brush strokes on a JPanel, which acts as a canvas
    - It has a menu bar with menu actions and a toolbar that lets the user choose tools like a brush, pen, eraser, etc
    - It allows the user to save an image as a pnt file (using a serialization algorithm) and export a pnt file to a png file
    - This project teaches us a lot about graphics, Java, Swing, serialization, deserialization, etc
3. [WordProcessor](https://github.com/ataylor89/WordProcessor)
    - This is an open-source word processor written in Java
    - It uses the Java Swing framework
    - It uses a JTextArea to display plain text
    - It has a cute class called ColorSample, which subclasses JButton, and creates an icon for choosing a foreground or background color
    - It has a class called PreferencesDialog, which subclasses JDialog, and creates a dialog for editing user preferences
    - It has a central class called WordProcessor, which subclasses JFrame, and builds the graphical user interface
    - It has settings (in the preferences dialog) for controlling font size, font name, foreground color, background color, etc
    - This project teaches us a lot about Java, Swing, and different Swing components (like JTextArea and JDialog)
4. [rsa](https://github.com/ataylor89/rsa)
    - This is an open-source implementation of the RSA encryption algorithm
    - The RSA encryption algorithm is an example of asymmetric key cryptography, which means that the encryption key is different from the decryption key
    - The RSA encryption algorithm is also an example of public key cryptography, which is really just a special case of asymmetric key cryptography, in which the encryption key is considered public and the decryption key is considered private
    - The RSA algorithm is very secure, and if the public key gets discovered, it cannot be used to decrypt messages, and a hacker must derive the private key from the public key in order to decrypt an encrypted message
    - In a symmetric key algorithm, like XOR, on the other hand, if a hacker discovers the encryption key, the hacker can use the encryption key to decrypt messages, since the encryption key and the decryption key are identical
    - The project contained within this repository uses a file called primetable.py to generate a prime table
    - The key generation algorithm chooses two distinct prime numbers, p and q, from the prime table
    - The key generation algorithm then calculates the (n, e, d) values based on p and q
    - n is the product of p and q; e is the encryption exponent; d is the decryption exponent
    - We use the formula c = m^e % n to calculate the cipher (c) for a Unicode code point (m)
    - We use the formula m = c^d % n to calculate the Unicode code point (m) for a cipher (c)
    - The formula c = m^e % n is used to encrypt a Unicode character
    - The formula m = c^d % n is used to decrypt a cipher
    - We loop through the characters in a string, encrypt each character, encode the cipher, and join the encodings to create an encrypted message (first we encrypt a code point and make it a cipher, then we encode the cipher, then we append the encoding to a string and the resulting string represents the encrypted message)
    - The rsa project uses a file called keytable.py to generate keys and add them to a key table
    - The project uses a file called keygen.py to generate a key pair (public and private) from the key table and write them to file
    - The encrypt.py module is used to encrypt a message given a public key
    - The decrypt.py module is used to decrypt an encrypted message given a private key
    - The util.py module has a method called power_mod_n which is used to efficiently calculate m^e % n and c^d % n
    - The project contained within this repository can be used to encrypt and decrypt messages using the RSA algorithm
    - This project teaches us a lot about public key cryptography, asymmetric key cryptography, and the RSA encryption algorithm
    - If Alice and Barbara want to exchange secure communications, then Alice gives Barbara her public key, and Barbara uses Alice's public key to encrypt her messages, and Barbara gives Alice her public key, and Alice uses Barbara's public key to encrypt her messages; then, Barbara uses her private key to decrypt Alice's messages, and Alice uses her private key to decrypt Barbara's messages
    - That's how it works... when Alice and Barbara exchange public keys, it is called a handshake, an RSA handshake
