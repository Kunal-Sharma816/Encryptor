# Secure File Storage System
## Team Members
1. Keshav Kabra(22bcs052)
2. Kunal Sharma(22bcs058)
3. Anish Raja(22bcs012)
4. Ketan Shamra(22bcs053)

## Overview
The Secure File Storage System provides a safe way to store sensitive files by encrypting them with the Advanced Encryption Standard (AES). This ensures that only authorized users with the correct decryption key can access the stored files.

## Features
- **AES Encryption**: Encrypts files with AES, providing a high level of data security.
- **User Authentication**: Authenticates users to restrict access to the file storage system.
- **Secure Key Management**: Manages encryption keys securely to prevent unauthorized access.
- **File Integrity Verification**: Verifies the integrity of files using hashing algorithms to detect tampering.
- **Access Logging**: Tracks all access attempts to maintain accountability.

## Security Benefits
This application protects against:
- **Data Breaches**: Ensures that files are unreadable in the event of unauthorized access.
- **Man-in-the-Middle Attacks**: Encrypts files before upload to prevent intercepted data from being readable.
- **Brute Force Attacks**: Uses strong AES encryption to prevent decryption by brute force.
- **Unauthorized Access**: Limits access to authenticated and authorized users only.
- **Tampering Detection**: Uses file integrity checks to detect any file modification.

## Getting Started

### Prerequisites
- Python 3.6+
- `pycryptodome` library for AES encryption
- SQLite or PostgreSQL for database management
- Flask or Django for backend (optional)

### Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/secure-file-storage.git
    ```
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

### Usage
1. Start the application:
    ```bash
    python app.py
    ```
2. Login or Register as a new user.
3. Upload files to the storage system (files are encrypted automatically).
4. Retrieve and decrypt files using your credentials and decryption key.

## Project Structure
- `app.py`: Main application logic.
- `encryption.py`: Encryption and decryption functions using AES.
- `models.py`: Database models for storing user information and files.
- `templates/`: HTML templates for the user interface.

## Technologies Used
- **Python**: Core programming language.
- **Flask/Django**: For web backend (optional).
- **SQLite/PostgreSQL**: Database for storing user credentials and encrypted files.
- **AES Encryption (PyCryptodome)**: Provides symmetric encryption.

## License
This project is licensed under the MIT License.

## Future Enhancements
- Implement two-factor authentication (2FA) for additional security.
- Integrate user-specific encryption keys for enhanced privacy.
- Add support for file sharing with public-key cryptography.

---

## Contributors
- **Your Name** - Initial Work



   
