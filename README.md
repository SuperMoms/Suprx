# SUPRX

![SUPRX Logo](assets/SuprX.png)

Official public release repo for SUPRX wallet downloads.

## Downloads

- [Windows wallet ZIP](downloads/suprx-win64.zip)
- [Linux archive](downloads/suprx-linux-x86_64-v1.0.1.tar.gz)
- [Windows checksums](SHA256SUMS.txt)
- [Linux checksum](SHA256SUMS-linux.txt)
- [Main site](https://suprx.supermoms.info/)
- [Audit page](https://suprx.supermoms.info/audit.html)
- [Proof page](https://suprx.supermoms.info/proof.html)
- [Explorer](https://api.suprx.supermoms.info/explorer/)
- Support: `suprx@supermoms.info`

## Current Release Files

### Windows

- File: `suprx-win64.zip`
- Built package date: `April 24, 2026`
- Size: `67,905,880 bytes`
- SHA256: `3db00c9949f9a25c82eb19eb27e3599f3a7092cdd3340db6712f912d9b4cf52b`

### Linux

- File: `suprx-linux-x86_64-v1.0.1.tar.gz`
- Built package date: `April 22, 2026`
- Size: `14,592,589 bytes`
- SHA256: `2d89778319362157dcd961e8247f6a3371c094da8ed38f1161a347427afde41a`

## What Is Inside

### Windows ZIP

- `suprx-qt.exe` - desktop wallet UI
- `suprxd.exe` - node daemon
- `suprx-cli.exe` - command line client
- `suprx-wallet.exe` - wallet tool
- `suprx-tx.exe` - transaction tool
- `suprx-util.exe` - utility tool
- `vc_redist.x64.exe` - Microsoft runtime installer
- `export_mobile_recovery_easy.bat` - helper to export wallet recovery data for a future mobile import

### Linux Archive

- `bin/suprx`
- `bin/suprxd`
- `bin/suprx-cli`
- `bin/suprx-wallet`
- `bin/suprx-tx`
- `bin/suprx-util`

## Quick Start

### Windows

1. Download `suprx-win64.zip`.
2. Unzip it into a normal folder such as `C:\SUPRX`.
3. Run `vc_redist.x64.exe` if Windows reports missing runtime files.
4. Open `suprx-qt.exe`.
5. Let the wallet sync before trusting balances.

### Linux

1. Download `suprx-linux-x86_64-v1.0.1.tar.gz`.
2. Extract it with `tar -xzf suprx-linux-x86_64-v1.0.1.tar.gz`.
3. Open the `bin` folder and run `./suprxd` or `./suprx`.
4. Let the node sync before trusting balances.

## Verify The Downloads

### Windows

```powershell
Get-FileHash .\suprx-win64.zip -Algorithm SHA256
```

Expected:

```text
3db00c9949f9a25c82eb19eb27e3599f3a7092cdd3340db6712f912d9b4cf52b
```

### Linux

```bash
sha256sum suprx-linux-x86_64-v1.0.1.tar.gz
```

Expected:

```text
2d89778319362157dcd961e8247f6a3371c094da8ed38f1161a347427afde41a
```

## Important Safety Notes

- This repo is only for public release files and public docs.
- It must never contain `wallet.dat`, private keys, mobile recovery exports, `.env` files, or node data.
- Anyone who gets wallet recovery exports can take the coins.
- Do not share files created by `export_mobile_recovery_easy.bat`.

## How SUPRX Fits Together

- `SUPRX` is the native SHA256d chain coin.
- `wSUPRX` is the Base-side wrapped token for trading and ecosystem utility.
- Public reserve proof: [api.suprx.supermoms.info/api/proof](https://api.suprx.supermoms.info/api/proof)
- Public bridge audit: [suprx.supermoms.info/audit.html](https://suprx.supermoms.info/audit.html)

## More Project Links

- [About SUPRX](https://suprx.supermoms.info/about.html)
- [Tokenomics](https://suprx.supermoms.info/tokenomics.html)
- [Litepaper](https://suprx.supermoms.info/litepaper.html)
- [Builder Bounties](https://suprx.supermoms.info/bounties.html)
