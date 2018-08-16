# Encryption with GPG

## Create a GPG key
```bash
gpg --full-gen-key
```

## Asymetric encryption
```bash
# Create a file
echo "This is some plain text" > file
# Encrypt
gpg -r <email> -e file
# Decrypt
gpg -d file.gpg
```

## Symmetric encryption
```bash
# Create a file
echo "This is some plain text" > new_file
# Encrypt
gpg --output encrypted_file --symmetric new_file
# Decrypt
gpg --output decrypted_file encrypted_file
```

