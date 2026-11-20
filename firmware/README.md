# Firmware

[English](README.md) | [简体中文](README_ZH.md)

Factory firmware for ESP32-S3_ePaper-3.97. The merged image is flashed at `0x0`.

| File | Purpose |
| --- | --- |
| `ESP32-S3-ePaper-3.97_FactoryOnly_20260314.bin` | Factory/demo firmware dated 2026-03-14 |

```bash
python -m pip install esptool
esptool.py --chip esp32s3 --port <PORT> erase_flash
esptool.py --chip esp32s3 --port <PORT> write_flash 0x0 ESP32-S3-ePaper-3.97_FactoryOnly_20260314.bin
```

