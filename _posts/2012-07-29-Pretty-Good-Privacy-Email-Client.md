---
layout: post
categories: [Java]
tags: [Java, cryptography, email, PGP]
excerpt_separator: <!--more-->

title: Pretty Good Privacy Email Client
---

**[Pretty Good Privacy](http://en.wikipedia.org/wiki/Pretty_Good_Privacy)** encryption was created by [Phil Zimmermann](http://en.wikipedia.org/wiki/Phil_Zimmermann) in 1991. It provides cryptographic privacy and authentication for data communication. Emails that are sent nowadays are not always secure, meaning that the content of an email could be seen and altered by someone other than the intended parties. Pretty Good Privacy will be able to offer more protection through the use of asymmetric encryption along with digital signature.  Each message is encrypted using RSA public key. Hence, only the intended recipient who has the private key would be able to decrypt the message. Furthermore, PGP ensures the authenticity of the message by allowing the sender to digitally sign the message.
<!--more-->

The goal of Pretty Good Privacy Client (PGPClient) is to provide a way for users to encrypt and decrypt their emails using a Java based application so that the contents of the email remain secure and safe. Moreover, PGPClient will help users to authenticate the email integrity by detecting whether it has been altered since it was completed. We want to provide an application that will interact with online keyservers (e.g. [MIT's PGP keyserver](http://pgp.mit.edu/)) in order to provide user authentication and message integrity. With this application, a user will be able to create an email, encrypt the content, sign it, and finally send the email. The user receiving the email will be able to decrypt the content and check the integrity of the message. The encryption algorithm that will be used is RSA with 1024-bit keys and PKCS#1 padding scheme.

{: .center}
![Pretty Good Privacy Encryption Diagram](/images/pgp_email/pgp_diagram.png)

PGPClient is written in Java. The GUI is based on Java Swing library. Currently, it only supports POP3 and has only been tested with GMail.

External Link
-------------

* [Project Website](https://github.com/mdandy/PGPClient)
