## SPI Pattern Generator – Logic Outline

1. Load input configuration (JSON)
2. Parse SPI mode (CPOL/CPHA) and pin mapping
3. For each instruction:
   - Write: Convert hex byte to bitstream
   - Read: Insert placeholder vectors
4. Assemble timing-accurate vector snippets
5. Output: pattern.vec

Example Output Format:
Pattern: SPI_Read_ID
  CS  SCLK  MOSI
  H    L     0
  H    H     0
