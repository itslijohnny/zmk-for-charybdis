zmk-config for charybdis (4x6)

## Build Configurations

This keyboard supports two usage modes. **You must flash different firmware depending on which mode you want to use.**

### Mode 1: Standalone (2 halves, no dongle)
- **Left half**: Peripheral
- **Right half**: Central (connects to PC via USB)
- **Flash firmware**:
  - Left: `charybdis_left_standalone.uf2`
  - Right: `charybdis_right_standalone.uf2`

### Mode 2: With Central Dongle (3 devices)
- **Left half**: Peripheral
- **Right half**: Peripheral
- **Dongle**: Central (connects to PC via USB, includes OLED display)
- **Flash firmware**:
  - Left: `charybdis_left_dongle.uf2`
  - Right: `charybdis_right_dongle.uf2`
  - Dongle: `charybdis_central_dongle_oled.uf2`

### Switching Between Modes

To switch from standalone to dongle mode (or vice versa):
1. Download the appropriate firmware builds from GitHub Actions
2. Reflash the **right half** with the correct version (`standalone` or `dongle`)
3. The left half firmware is identical for both modes, but separate builds are provided for clarity

**Note**: The trackball is physically located on the right half and functions in both modes. Input is automatically forwarded from peripherals to the central device.
