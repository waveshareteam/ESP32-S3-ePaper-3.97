# 固件

[English](README.md) | [简体中文](README_ZH.md)

ESP32-S3_ePaper-3.97 出厂固件。合并镜像从 `0x0` 地址开始烧录。

| 文件 | 用途 |
| --- | --- |
| `ESP32-S3-ePaper-3.97_FactoryOnly_20260314.bin` | 2026-03-14 出厂演示固件 |

```bash
python -m pip install esptool
esptool.py --chip esp32s3 --port <PORT> erase_flash
esptool.py --chip esp32s3 --port <PORT> write_flash 0x0 ESP32-S3-ePaper-3.97_FactoryOnly_20260314.bin
```

