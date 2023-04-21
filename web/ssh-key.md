# SSH key generation

## 1. SSH Key Generation

[Generating a new SSH key and adding it to the ssh-agent](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
```
ssh-keygen -t ed25519 -C "your_email@example.com"
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

## 2. Signing Commits

[About commit signature verification](https://docs.github.com/en/authentication/managing-commit-signature-verification/about-commit-signature-verification)
```
# git version must be 3.4 or above
git config --global user.signingkey /PATH/TO/.SSH/KEY.PUB
git config --global gpg.format ssh
git commit -S -m "YOUR_COMMIT_MESSAGE"
```