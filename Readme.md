# pspdecrypt
A quick and *dirty* tool to decrypt PSP binaries, and also PSP updaters (PSAR format)

Licensed under GPLv3

Decryption code copied from [ppsspp](https://github.com/hrydgard/ppsspp/), making use of libkirk by draan

KL3E & KL4E implementation and PSAR extraction by artart78

## Usage
This project is made up of two utilities: `pspdecrypt` and `psardecrypt`.

`pspdecrypt` is a one-shot utility to decrypt a single `prx` with a `~PSP` ELF header.

`psardecrypt` will extract the contents of a `PSAR`, decrypting and decompressing each asset as required. Will also extract IPL stages 1-3 when possible.

## Release Notes
### 0.8
 * Adds KL4E & KL4E decompression support for PSAR contents
 * Adds `PSAR` support
 * Extracts most public FW, older JigKick payloads, and most TT FW
 
### Initial release (unversioned)
 * Decrypts `PRX` files
