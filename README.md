# PairUX APT Repository

APT repository for PairUX - Debian/Ubuntu packages.

## Installation

```bash
# Add the GPG key
curl -fsSL https://raw.githubusercontent.com/profullstack/pairux-apt/main/pairux.gpg | sudo gpg --dearmor -o /usr/share/keyrings/pairux-archive-keyring.gpg

# Add the repository
echo "deb [signed-by=/usr/share/keyrings/pairux-archive-keyring.gpg] https://profullstack.github.io/pairux-apt stable main" | sudo tee /etc/apt/sources.list.d/pairux.list

# Update and install
sudo apt update
sudo apt install pairux
```

## Manual Download

You can also download `.deb` packages directly from [GitHub Releases](https://github.com/profullstack/pairux.com/releases).

## Repository Structure

- `pool/` - Package files
- `dists/` - Distribution metadata
- `pairux.gpg` - Repository GPG public key

## License

MIT License - see [pairux.com](https://github.com/profullstack/pairux.com) for details.
