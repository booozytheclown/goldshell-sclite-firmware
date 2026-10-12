# Goldshell SC Lite Firmware Research

Independent community research into the Goldshell SC Lite ASIC miner firmware, including reverse engineering, hardware configuration, thermal management, and firmware upgrade mechanisms.

## Stock Firmware 2.2.0

| Property | Value |
|---|---|
| Manufacturer | Goldshell |
| Model | SC Lite |
| Firmware | 2.2.0 |
| Control Board | MCB_V4_3 |
| Algorithm | Blake2b |
| Format | TGZ firmware archive |

**[Download Firmware Release v2.2.0](https://github.com/booozytheclown/goldshell-sclite-firmware/releases/tag/stock-2.2.0)**

### SHA-256 Verification

Firmware: `burn-Goldshell-SCLITE_MCB_V4_3-2.2.0.tgz`

Expected SHA-256:

`1c84eebc9ca1b75e69cb729f64f6fb7dbc59a30bd8ee42049e6186de145eb433`

Linux verification:

```bash
sha256sum -c burn-Goldshell-SCLITE_MCB_V4_3-2.2.0.tgz.sha256
```

Windows PowerShell verification:

```powershell
Get-FileHash -LiteralPath ".\burn-Goldshell-SCLITE_MCB_V4_3-2.2.0.tgz" -Algorithm SHA256
```

The SHA-256 checksum was verified against a local copy of the firmware prior to publication. This establishes integrity relative to the published checksum, not independent manufacturer authenticity.

## Research Objectives

- Reverse engineer the original firmware.
- Document the embedded Linux filesystem and firmware architecture.
- Investigate firmware validation, signing, upgrading, and recovery.
- Research fan speeds, thermal regulation, and miner hardware controls.
- Explore configuration and performance improvements.
- Share reproducible technical findings and encourage community development.

## Contributing

Community contributions are welcome!

Use GitHub Issues to report discoveries, document firmware behavior, or propose improvements.

Submit Pull Requests for research documentation, independently developed tools, and reproducible analysis.

Please avoid publishing passwords, private keys, device credentials, or personally identifiable information.

## Disclaimer

This project is independent and is not affiliated with or endorsed by Goldshell.

Original firmware and manufacturer documentation remain subject to their respective intellectual property rights.

Firmware modification and flashing carry risks, including hardware damage and device failure. Experimental work should be performed with appropriate safeguards.

This repository does not guarantee firmware safety, authenticity, or suitability for production hardware.
