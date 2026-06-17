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


Категория: Безопасность (Security)

[ ] Настройка SSH-авторизации только по ключам, отключение паролей.

[ ] Ограничение прав доступа и базовая настройка Firewall.

[ ] Базовая настройка Git (Global Config) для системы.

Категория: Производительность (System Optimization)

[ ] Оптимизация питания: фиксация CPU в режиме performance.

[ ] Активация аппаратного Watchdog.

[ ] Защита SD-карты от износа: перенос /var/log в RAM (tmpfs).

[ ] Настройка GPU Memory Split для задач с видео.

Категория: Сеть и периферия (Hardware & Connectivity)

[ ] Отключение энергосбережения Wi-Fi (NetworkManager).

[ ] Настройка статического IP.

[ ] Активация аппаратных шин: I2C, UART, SPI.

[ ] Конфигурация интерфейса CAN (can0).
