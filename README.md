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
    - To be continued... I might push these changes before I finish writing the file
