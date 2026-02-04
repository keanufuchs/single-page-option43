# Cisco DHCP Option 43 Builder

Single-page web app that generates Cisco DHCP Option 43 hex for classic WLC discovery (F1) and Fast Offline Migration (F3), plus IOS / IOS-XE DHCP pool configs.

## Features
- F1 and F3 Option 43 generation with correct length calculation
- F3 AP mode byte (Meraki/Catalyst) enforcement
- Byte-by-byte hex breakdown with hover tooltips
- IOS / IOS-XE DHCP pool config output
- Client-side only (no backend)

## Usage
1. Open `index.html` in a browser.
2. Select the DHCP mode (F1 or F3).
3. Enter the Management VLAN subnet in CIDR format.
4. Enter the WLC IPv4 address.
5. Copy the hex output or the full IOS config.

## Notes
- F3 requires the AP mode byte (Meraki `01`, Catalyst `02`).
- IOS config output uses the CIDR input to derive network and mask.

## Files
- `index.html`: Application UI and logic
- `README.md`: Project overview
