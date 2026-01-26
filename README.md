# PairUX APT Repository

## Installation

```bash
# Add GPG key
curl -fsSL https://profullstack.github.io/pairux-apt/pairux.gpg | sudo gpg --dearmor -o /usr/share/keyrings/pairux.gpg

# Add repository
echo "deb [signed-by=/usr/share/keyrings/pairux.gpg] https://profullstack.github.io/pairux-apt stable main" | sudo tee /etc/apt/sources.list.d/pairux.list

# Install
sudo apt update
sudo apt install pairux
```
