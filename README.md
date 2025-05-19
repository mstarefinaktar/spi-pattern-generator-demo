# SPI Pattern Generator (Concept Demo)

This project outlines a C++ post-processing script developed for SPI protocol pattern generation on ATE platforms (e.g., Advantest V93000).

⚠️ This is a structural and conceptual demo — full proprietary code is not shared.

## Features
- Supports SPI mode selection (CPOL/CPHA)
- Generates SPI vectors for write/read commands
- Outputs example vector fragments for integration with pattern tools

## Example Flow
```json
{
  "mode": 0,
  "cs_pin": "CS",
  "sclk_pin": "SCLK",
  "mosi_pin": "MOSI",
  "sequence": [
    {"type": "write", "data": "0x9F"},
    {"type": "read", "length": 3}
  ]
}
```

Result: Generates pattern for SPI read ID command.

