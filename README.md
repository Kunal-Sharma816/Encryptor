# Secure File Storage System

## Overview
The Secure File Storage System is a web application built with a full-stack setup to ensure the secure storage of sensitive files. Files are encrypted on the client side using AES encryption, making sure that only authorized users with the decryption key can access stored files.

## Features
- **AES Encryption (Client-Side)**: Encrypts files before they reach the server, providing additional security.
- **User Authentication**: Verifies user credentials to restrict access to the storage system.
- **MySQL Database**: Efficiently stores encrypted files and metadata.
- **Access Logging**: Maintains a record of access attempts, ensuring transparency and accountability.

## Security Benefits
This application provides protection against:
- **Data Breaches**: Client-side encryption keeps data secure even if the database is compromised.
- **Unauthorized Access**: Limits access to authenticated users with proper credentials.
- **Man-in-the-Middle Attacks**: Files are encrypted on the client side, so intercepted data remains unreadable.

## Technology Stack
- **Frontend**: Next.js, React.js, Tailwind CSS
- **Backend**: Express.js, MySQL, JavaScript (AES Encryption)

## Getting Started

### Prerequisites
- Node.js and npm installed
- MySQL installed and running
- Environment file for database configuration (e.g., `.env`)

### Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/secure-file-storage.git
    ```
2. Navigate to the project directory:
    ```bash
    cd secure-file-storage
    ```
3. Install dependencies:
    ```bash
    npm install
    ```
4. Configure your MySQL database in the `.env` file:
    ```
    DB_HOST=your_host
    DB_USER=your_user
    DB_PASSWORD=your_password
    DB_NAME=your_database
    ```
5. Start the backend server:
    ```bash
    npm run server
    ```
6. Start the Next.js frontend server:
    ```bash
    npm run dev
    ```

### Usage
1. Register as a new user or log in to access your secure file storage.
2. Upload files; each file is encrypted before being sent to the server.
3. Download and decrypt files with the correct credentials.

## Project Structure
- `frontend/`: Next.js, React.js frontend with Tailwind CSS styling
- `backend/`: Express.js server and API endpoints
- `encryption/`: AES encryption module implemented in JavaScript
- `database/`: MySQL setup and migrations

## Future Enhancements
- Integrate two-factor authentication (2FA) for an extra layer of security.
- Implement user-specific keys for finer-grained encryption control.
- Support for file sharing through public-key cryptography.

## License
This project is licensed under the MIT License.

## Contributors
- **Your Name** - Initial Work

