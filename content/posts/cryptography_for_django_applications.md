---
Category: 'DjangoCon 2012'
Copyright: 'Creative Commons Attribution license (reuse allowed'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=pWCAADXd-DI"'
Speakers: [Erik Labianca]
Tags: [cryptography, django]
ThumbnailUrl: 'http://i.ytimg.com/vi/pWCAADXd-DI/hqdefault.jpg'
Title: '"Cryptography for Django Applications"'
date: '2012-09-05'
---
# Introduction

The web is a hostile place, and isn't showing any signs of becoming less so.
In order to mitigate this, many developers turn to cryptography.
Unfortunately, cryptography can be complicated, and is easily circumvented if
not properly handled. This presentation will provide an introduction to
cryptographic tools available to Python/Django applications, appropriate use
cases for each, proper usage, and operational concerns necessary to operate in
a certified environment. Finally, we will also demonstrate a reusable
application that wraps this all up, providing secure key-management
capabilities to a running Django environment via the Django admin.

# Why Encrypt?

# Rules of Encryption

  * Don't do it if you don't need it.
  * Don't write your own.
  * Understand what you're doing if you do.

# When to encrypt?

## Understand what you're protecting

  * Data
  * User records
  * Code
  * Systems

## Understand your attack vectors

  * Data (backups, revision control)
  * Systems
  * Application
  * Transport
  * Client

## Understand the types of encryption you might use:

  * Hashing

### Passwords are a special case. Use a key derivation function

  * PBKDF2 – Upgrade to Django 1.4!

### Algorithms

  * MD5 - fine as a checksum. not fine as a cryptographic hash.
  * SHA1 - fine as a checksum. becoming less fine as a cryptographic hash every day
  * SHA2 - so far so good. use as many bits as you can handle.

## Symmetric Encryption

  * Fast
  * Reversible

### Algorithms

  * Caesar Cipher (for fun puzzles)
  * DES (don't use)
  * AES (certified)
  * Blowfish

## Asymmetric Encryption

  * Slow
  * One-way

### Algorithms

  * RSA
  * DSA

#### Uses

##### Signing

###### Web of Trust

  * PGP

###### PKI

##### Encryption

  * PGP
  * SSL
  * TLS

# Doing it right

## Use known-good algorithms

  * AES-256
  * SHA2
  * RSA
  * DSA

## Use known-good implementations

  * Open Source is good

## Extra Credit

  * FIPS 140 certified implementations
  * FIPS 140 / NIST configurations

## Transport (always use HTTPS)

  * Use good algorithms AES-256

## At Rest (insecure servers or backups)

  * Understand the ramifications of key management

# Examples

## Hashing

  * Use a key-derivation function

### Don't be linked-in

  * Salt your hashes (with a secret). 
  * Salt and pepper your hashes if possible (with a known unique value)

## SSL

  * Forced connections
  * Making the application aware
  * Hardened cipher selection

### Robust PKI

  * Client authentication
  * SSL Test Page

## Asymmetric Encryption

### Key Management

  * Using GPG Agent
  * GPG Manager App

### PGP Files

## Symmetric Encryption

### Key Management

  * Use Asymmetric Encryption

### Use a unique Initialization Vector if possible

  * LoopBack Devices

