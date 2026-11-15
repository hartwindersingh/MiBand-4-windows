# MiBand 4 Windows

Windows-focused tools and research for connecting to the Xiaomi Mi Smart Band 4 over Bluetooth Low Energy (BLE).

## Repository layout

The reference projects below are included as Git submodules. Two now point to copies under the `hartwindersingh` account, so changes to the original repositories will not automatically change these pinned copies. The heart-rate reference remains linked to its upstream repository because a personal copy has not yet been created.

- `vendor/miband4-protocol` — [hartwindersingh/miband4-f1](https://github.com/hartwindersingh/miband4-f1): personal copy of the Mi Band 4 BLE protocol/authentication reference. Originally from [satcar77/miband4](https://github.com/satcar77/miband4); Linux-oriented, so Windows adaptation is required.
- `vendor/miband-hrx-accelerometer` — [hartwindersingh/MiBand_HRX](https://github.com/hartwindersingh/MiBand_HRX): personal copy of accelerometer research for Mi Band HRX hardware. Compatibility with Mi Band 4 is unverified.
- `vendor/hrs-heartrate-osc` — [wwtssu/hrs-heartrate-osc](https://github.com/wwtssu/hrs-heartrate-osc): upstream Windows 10/11 heart-rate monitoring reference for Mi Band 2/3/4/5; it does not provide raw accelerometer streaming.

## Clone with references

```powershell
git clone --recurse-submodules https://github.com/hartwindersingh/MiBand-4-windows.git
```

To initialise submodules after a normal clone:

```powershell
git submodule update --init --recursive
```

## Important

No claim is made that the HRX accelerometer code works on Mi Band 4. The next engineering step is to validate the Band 4 GATT services, authentication, and motion-data characteristics on the actual device. Keep any device authentication key local; do not commit it.

## Credits and licensing

The personal copies retain their original history and attribution. Each project remains subject to its own license and copyright notices. Review the applicable license before redistributing or modifying code. The personal copies will not receive upstream changes unless you explicitly sync them.
