# Threema

## Servers

### Chat Server

### Directory Server 

### Media Server

## Security 

### Verification Layer

- **Red (level 1):** Public key from the server. No matching contact and therefore the user cannot be sure that the person is who they claim to be in their messages.
- **Orange (level 2):** Matching contact. The user can be reasonably sure that the person is who they claim to be.
- **Green (level 3):** The user has personally verified the ID and public key of the contact by scanning their QR code. The user can be very sure that messages from this contact were really written by the person that they indicate.

### End-to-end encryption layer

Between the sender and the recipient.

### Transport layer

Each end-to-end encrypted message is encrypted again for transport between the client and the server, in order to protect the header information.

### Local Storage

### Call Encryption

DTLS ciphersuites - in that order
- TLS_ECDHE_ECDSA_WITH_CHACHA20_POLY1305_SHA256 (0xcca9)
- TLS_ECDHE_ECDSA_WITH_AES_256_GCM_SHA384 (0xc02c)
- TLS_ECDHE_ECDSA_WITH_AES_128_GCM_SHA256 (0xc02b)

SRTP ciphersuites - in that order
- SRTP_AEAD_AES_256_GCM (0x0008)
- SRTP_AEAD_AES_128_GCM (0x0007)
- SRTP_AES128_CM_HMAC_SHA1_80 (0x0001)

### Threema Safe

- Threema ID
- Private key
- Profile information (Nickname, Profile photo, Linked email address and phone number)
- Contact list (Contact Threema ID, Public key, Name, Verification level)
- Group definitions (Group ID, Creator, Group name, List of members)
- Distribution lists (Name, List of members)
- App settings

## Summary 

| Algorithm | Name |
|:---------:|:----:|
| Elliptic Curve Cryptography | Curve25519 | 
| Message Authentication Code | Poly1305 | 
| PRNG | iOS : /dev/random - Fortuna <br/> Android : /dev/random - Linux PRNG |
| Audio Encoding | Opus codec at 48 kHz (CBR) |
| Video Encoding | VP9, VP8 or H.264 |

## Threema Application 

### General - Application

| Application Name | Threema |
|:----------------:|:-------:|
| Developers | Threema GmbH | 
| Released | December 2012 |
| Package Name | ch.threema.app |
| Process Name | ch.threema.app |

### General - Android  

| Platform | Android |
|:--------:|:-------:|
| Version Name | 4.72 |
| Version Code | 3000738 |
| System Application | No | 
| UID | 10348 |
| Installer | com.android.vending |
| Application Source | Google Play |
| Target SDK | 30 |
| Target Version | Android 11 |
| Minimal SDK | 21 |
| Min Version | Android 5.0 Lollipop | 
| APK Size | 28 MB |

### Certificate 

| Signature Algorithm | SHA256withRSA |
|:-------------------:|:-------------:|
| Valid From | 28/04/2013 1:42 AM |
| Valid To | 13/09/2040 1:42 AM |

### Components 

| Component Name | Count  |
|:--------------:|:------:|
| Activity | 98 |
| Broadcast Receiver | 16 |
| Service | 30 |
| Content Provider | 4 |

