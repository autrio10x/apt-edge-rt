# apt-edge-rt

Public apt archive for Keystone. App source stays in the private `autrio10x/keystone` repo.

```bash
sudo mkdir -p /etc/apt/keyrings
curl -fsSL https://autrio10x.github.io/apt-edge-rt/keystone.gpg \
  | sudo tee /etc/apt/keyrings/keystone.gpg >/dev/null
echo "deb [signed-by=/etc/apt/keyrings/keystone.gpg] https://autrio10x.github.io/apt-edge-rt stable main" \
  | sudo tee /etc/apt/sources.list.d/keystone.list
sudo apt update
sudo apt install keystone
```
