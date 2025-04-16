# fpvKit

---

## 📂 Структура проекта

```
fpv-drone-project/
├── README.md
├── docs/
│   ├── wiring.md
│   ├── uart-setup.md
│   ├── vtx-camera.md
│   └── elrs.md
├── diffs/
│   ├── 2025-04-15_initial.diff
│   ├── 2025-04-16_gps_added.diff
│   └── ...
├── logs/
│   └── blackbox_2025-04-16.bbl
└── firmware/
    └── INAV_SPEDIXF405_8.0.1.hex
```

---

## 📋 Базовая информация

- **FC:** Spedix F4 55A  
- **ESC:** 4-in-1  
- **RX:** ELRS 2.4 GHz (CRSF)  
- **Camera:** Caddx EOS2 Turbo  
- **VTX:** AKK Dominator 2.0  
- **Protocol:** DSHOT300  
- **Firmware:** INAV 8.0.1

---

## ⚙️ Полезные команды INAV CLI

```bash
diff all
status
resource
save
set motor_pwm_protocol = DSHOT300
```

## 🐧 Linux утилиты

```bash
lsusb
dfu-util -l
screen /dev/ttyACM0 115200
ls /dev/tty*
dmesg | grep tty
```

---

## 🧭 Для чего нужен этот репозиторий

- Хранить `diff all` для откатов и истории
- Документировать каждый шаг: wiring, UART, конфигурацию
- Делать backup прошивок и логов
- Делиться с сообществом

---

## 📄 Лицензия

MIT — свободно использовать и адаптировать.-
