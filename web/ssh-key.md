# SSH key generation

## 1. Fast and Simple

```
# SSH Key Generation
ssh-keygen -t ed25519 -C "your_email@example.com"
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

## 2. Detailed

[Generating a new SSH key and adding it to the ssh-agent](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
[About commit signature verification](https://docs.github.com/en/authentication/managing-commit-signature-verification/about-commit-signature-verification)