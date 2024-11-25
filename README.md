
### ⬇️ Install

Run these commands:

```
nix-shell -p git vim
git clone https://github.com/abdallahghdiri/dotfiles
cd dotfiles
nixos-generate-config --show-hardware-config > hosts/default/hardware-configuration.nix
NIX_CONFIG="experimental-features = nix-command flakes" sudo nixos-rebuild switch --flake .#default
```