# keys
Public keys which are basically... Public

Since github publicly exposes github user's public key, then might as well do the same for easier query :p

List with shortened urls:
- pub.key - https://git.io/fA5Qm


To Append

- Already logged in: 
```bash
curl -Ls https://git.io/fA5Qm >> ~/.ssh/authorized_keys
```

- Not logged in:
```bash
ssh user@server "curl -Ls https://git.io/fA5Qm >> ~/.ssh/authorized_keys"
```

Check Existing
```bash
cat ~/.ssh/authorized_keys | grep $(curl -Ls https://git.io/fA5Qm)
```
