# MiBand 4 Windows

Windows-focused tools and research for connecting to the Xiaomi Mi Smart Band 4 over Bluetooth Low Energy (BLE).

## External research repositories

The following projects are linked as Git submodules so their upstream history, authorship, and licenses remain intact. They are reference implementations, not yet integrated or verified as compatible with this Windows application.

- `vendor/miband4-protocol` — [satcar77/miband4](https://github.com/satcar77/miband4): Mi Band 4 BLE protocol and authentication reference (Linux-oriented; Windows adaptation required).
- `vendor/miband-hrx-accelerometer` — [4lhc/MiBand_HRX](https://github.com/4lhc/MiBand_HRX): accelerometer research for Mi Band HRX hardware; compatibility with Mi Band 4 is unverified.
- `vendor/hrs-heartrate-osc` — [wwtssu/hrs-heartrate-osc](https://github.com/wwtssu/hrs-heartrate-osc): Windows 10/11 heart-rate monitoring reference for Mi Band 2/3/4/5; it does not provide raw accelerometer streaming.

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

Each linked project remains under its own upstream license and copyright notices. Review each upstream repository's license before redistributing or modifying its code.