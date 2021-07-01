# Django Settings Best Practices, SSH

Tips and code examples for configuring settings.py.

https://djangostars.com/blog/configuring-django-settings-best-practices/

> "Django Settings: Best practices
> 1. Keep settings in environment variables.
> 2. Write default values for production configuration (excluding secret keys and tokens).
> 3. Don’t hardcode sensitive settings, and don’t put them in VCS.
> 4. Split settings into groups: Django, third-party, project.
> 5. Follow naming conventions for custom (project) settings.
"

# SSH

https://www.hostinger.com/tutorials/ssh-tutorial-how-does-ssh-work

> "SSH, or Secure Shell, is a remote administration protocol that allows users to control and modify their remote servers over the Internet."

### SSH and Encryption

Refer to read18 for more on encryption:
[read18](/Users/skylerjohnson/Documents/projects/codefellows/code401python/reading-notes/401python/read18.md)

1. Symmetrical encryption
2. Asymmetrical encryption
3. Hashing.

> "**Symmetric encryption** is a form of encryption where a secret key is used for both encryption and decryption of a message by both the client and the host. Symmetrical encryption is often called shared key or shared secret encryption. "

> "Unlike symmetrical encryption, **asymmetrical encryption** uses two separate keys for encryption and decryption. These two keys are known as the public key and the private key. Together, both these keys form a public-private key pair. The strength of the entire connection lies in the fact that the private key is never revealed, as it is the only component capable of decrypting messages that were encrypted using its own public key."

> "**One-way hashing** is another form of cryptography used in Secure Shell Connections. One-way-hash functions differ from the above two forms of encryption in the sense that they are never meant to be decrypted. They generate a unique value of a fixed length for each input that shows no clear trend which can exploited. This makes them practically impossible to reverse. SSH uses hashes to verify the authenticity of messages. This is done using HMACs, or Hash-based Message Authentication Codes. This ensures that the command received is not tampered with in any way."

# Whitenoise

http://whitenoise.evans.io/en/stable/

# Infrastructure as a service

https://en.wikipedia.org/wiki/Infrastructure_as_a_service

# Platform as a service

https://en.wikipedia.org/wiki/Platform_as_a_service

# CORS

https://en.m.wikipedia.org/wiki/Cross-origin_resource_sharing


[code401 Reading Notes](../401Python/code401Table.md)
