# Sonic Signature

Environment-based authentication system that uses acoustic room signatures to enhance cybersecurity.

## Problem Statement
Traditional authentication methods such as passwords, OTPs, and biometrics can be vulnerable to phishing, interception, and spoofing attacks. There is a need for an additional security layer that verifies not just the user, but also the environment from which access is requested.

## Solution
Sonic Signature introduces an authentication method based on the unique acoustic fingerprint of a room. When a user attempts to log in, the system emits a high-frequency tone through the device speaker. The microphone records how the sound reflects from walls, furniture, and objects in the room.

The captured audio signal is analyzed using signal processing techniques such as Fast Fourier Transform (FFT) to generate an acoustic signature of the environment. This signature is then compared with the stored room profile to grant or deny access.

## Key Features
- Environment-based authentication
- Acoustic fingerprint generation
- High-frequency authentication tone
- Echo capture using device microphone
- FFT-based audio signal analysis
- Pattern matching with stored room signatures
- Access control based on signature match

## System Workflow
1. User initiates login.
2. System emits a high-frequency authentication tone.
3. Device microphone captures room echo reflections.
4. Audio signals are processed using FFT.
5. Acoustic fingerprint is generated.
6. System compares fingerprint with stored room signature.
7. Access is granted or denied.

## Technology Stack
- Web Audio API (Audio capture & tone generation)
- Python (NumPy, SciPy) for signal processing
- Fast Fourier Transform (FFT)
- Node.js / Flask backend
- PostgreSQL / MongoDB database

## Potential Applications
- Corporate office authentication
- Secure laboratory access
- Data center security
- Smart home access control

## Hackathon
Project submitted for **Hack Break – Generative AI & Cybersecurity Innovation Challenge (IIT Bombay)**.
