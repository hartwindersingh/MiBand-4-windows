# MiBand 4 Windows

Windows-focused tools and research for connecting to the Xiaomi Mi Smart Band 4 over Bluetooth Low Energy (BLE).

## Repository layout

The reference projects below are included as Git submodules. All three submodule URLs now point to repositories under the `hartwindersingh` account. Their code remains pinned to specific commits; changes in upstream repositories will not automatically change these copies.

- `vendor/miband4-protocol` — [hartwindersingh/miband4-f1](https://github.com/hartwindersingh/miband4-f1): personal copy of the Mi Band 4 BLE protocol/authentication reference. Originally from [satcar77/miband4](https://github.com/satcar77/miband4); Linux-oriented, so Windows adaptation is required.
- `vendor/miband-hrx-accelerometer` — [hartwindersingh/MiBand_HRX](https://github.com/hartwindersingh/MiBand_HRX): personal copy of accelerometer research for Mi Band HRX hardware. Compatibility with Mi Band 4 is unverified.
- `vendor/hrs-heartrate-osc` — [hartwindersingh/Miband-heartrate-osc](https://github.com/hartwindersingh/Miband-heartrate-osc): personal copy of the Windows heart-rate monitor for Mi Band 2/3/4/5 and HRS devices. It provides heart-rate data and OSC integration, not raw accelerometer streaming. Originally from [wwtssu/hrs-heartrate-osc](https://github.com/wwtssu/hrs-heartrate-osc).

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

The personal copies retain their original attribution and license obligations. Review each project's license and notices before modifying or redistributing its code. Personal copies will not receive upstream changes unless you explicitly sync them.
