# File Encryption and Decryption

This repository contains scripts to encrypt and decrypt files using the `cryptography.fernet` module in Python.
## Important Note : Use Linux 
use cmd - `sudo su` (run it as root user)

## Files

- `voldemart.py`: Script to encrypt files.
- `decrypt.py`: Script to decrypt files.
- `thekey.key`: The key file used for encryption and decryption.

## Requirements

- Python 3.x
- `cryptography` module

You can install the `cryptography` module using pip:
```sh
pip install cryptography
```

## Usage

### Encryption

To encrypt files, run the `voldemart.py` script:
```sh
python3 voldemart.py
```

### Decryption

To decrypt files, run the `decrypt.py` script:
```sh
python3 decrypt.py
```

### Important Note

If you run the `voldemart.py` script multiple times, it will generate a new encryption key each time, which will make previously encrypted files undecryptable using the `decrypt.py` script.

### Solution

To avoid generating a new key each time, follow these steps:

1. **Check if `thekey.key` already exists before generating a new key**:
    - Modify `voldemart.py` to check for the existence of `thekey.key` before creating a new key.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### Key Points:
```
1. **Explanation of Files**: Describes the purpose of each file in the repository.
2. **Requirements**: Lists the requirements and how to install them.
3. **Usage Instructions**: Provides instructions for running the encryption and decryption scripts.
4. **Important Note and Solution**: Explains the issue with generating a new key on repeated encryption and provides a solution by modifying `voldemart.py` to reuse the existing key.
5. **License**: Includes a placeholder for the project's license information.
