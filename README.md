# SUPRX

![SUPRX Logo](assets/SuprX.png)

Official public release repo for SUPRX wallet downloads.

## Downloads

- [Windows wallet ZIP](downloads/suprx-win64.zip)
- [Linux archive](downloads/suprx-linux-x86_64-v1.0.8.tar.gz)
- [Windows checksums](SHA256SUMS.txt)
- [Linux checksum](SHA256SUMS-linux.txt)
- [Main site](https://api.suprx.supermoms.info/)
- [Audit page](https://api.suprx.supermoms.info/audit.html)
- [Proof page](https://api.suprx.supermoms.info/proof.html)
- [Explorer](https://api.suprx.supermoms.info/explorer/)
- Support: `suprx@supermoms.info`

## Current Release Files

### Windows

- File: `suprx-win64.zip`
- Built package date: `June 22, 2026`
- Size: `67,892,005 bytes`
- SHA256: `619d9a665b37a5092d5615555e3e35d34e397f851bb68ca0e04cf63d2a8eef91`

### Linux

- File: `suprx-linux-x86_64-v1.0.8.tar.gz`
- Built package date: `June 15, 2026`
- Size: `16,867,567 bytes`
- SHA256: `17ed8d1b36b58279d2fa793ae0572135fc67ff6b8611f7676f1fb4d4f4605642`

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

1. Download `suprx-linux-x86_64-v1.0.8.tar.gz`.
2. Extract it with `tar -xzf suprx-linux-x86_64-v1.0.8.tar.gz`.
3. Open the `bin` folder and run `./suprxd` or `./suprx`.
4. Let the node sync before trusting balances.

## Verify The Downloads

### Windows

```powershell
Get-FileHash .\suprx-win64.zip -Algorithm SHA256
```

Expected:

```text
619d9a665b37a5092d5615555e3e35d34e397f851bb68ca0e04cf63d2a8eef91
```

### Linux

```bash
sha256sum suprx-linux-x86_64-v1.0.8.tar.gz
```

Expected:

```text
17ed8d1b36b58279d2fa793ae0572135fc67ff6b8611f7676f1fb4d4f4605642
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
- Public bridge audit: [api.suprx.supermoms.info/audit.html](https://api.suprx.supermoms.info/audit.html)

## More Project Links

- [About SUPRX](https://api.suprx.supermoms.info/about.html)
- [Tokenomics](https://api.suprx.supermoms.info/tokenomics.html)
- [Litepaper](https://api.suprx.supermoms.info/litepaper.html)
- [Builder Bounties](https://api.suprx.supermoms.info/bounties.html)
