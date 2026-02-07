zmk-config for charybdis (4x6)

## Configuration

This keyboard uses a 3-device setup with a central dongle:

- **Left half**: Peripheral
- **Right half**: Peripheral (with trackball)
- **Dongle**: Central (connects to PC via USB, includes OLED display)

### Flashing Firmware

Flash the firmware from GitHub Actions to each device:

1. **Left half**: `nice_nano_v2-charybdis_left-zmk.uf2`
2. **Right half**: `nice_nano_v2-charybdis_right-zmk.uf2`
3. **Dongle**: `nice_nano_v2-charybdis_central_dongle_dongle_display-zmk.uf2`

**Note**: The trackball is physically located on the right half. Input from both peripherals (including trackball events) is automatically forwarded to the central dongle, which then sends all data to your PC.
