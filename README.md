# rpi4b-base-system
Загрузочная флешка для Raspberry PI 4B+

rpi-base-system/
├── scripts/              # Bash-скрипты для быстрой настройки (Этапы 1-4)
│   ├── 01_security.sh    # SSH, ключи, отключение паролей
│   ├── 02_system.sh      # Watchdog, CPU performance, tmpfs (логи)
│   ├── 03_network.sh     # Static IP, отключение энергосбережения Wi-Fi
│   └── 04_peripherals.sh # I2C, UART, SPI, CAN-интерфейс
├── configs/              # Шаблоны конфигов (которые вы будете копировать)
│   ├── config.txt        # Для активации шин RPi
│   ├── cmdline.txt
│   └── sshd_config
├── docs/                 # Документация по железу
└── README.md             # Инструкция: "Как развернуть базу на чистой Ubuntu 26.04"
