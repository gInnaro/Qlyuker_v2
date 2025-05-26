[![Static Badge](https://img.shields.io/badge/Telegram-Bot%20Link-Link?style=for-the-badge&logo=Telegram&logoColor=white&logoSize=auto&color=blue)](https://t.me/qlyukerbot/start?startapp=bro-1197825376)
[![Static Badge](https://img.shields.io/badge/Telegram-Channel-Link?style=for-the-badge&logo=Telegram&logoColor=white&logoSize=auto&color=blue)](https://t.me/CyberToolz)

# Бот для Qlyuker v2

![start--qlyuker](https://github.com/user-attachments/assets/5c00a76b-946d-46a6-9243-06112b3dca35)


# 🔥🔥 Используйте Python версии 3.10 - 3.11.5 🔥🔥

> 🇪🇳 README in english available [[here](https://github.com/Cybertat1on/Qlyuker/blob/main/README-EN.md)]

## Функционал  
|                   Функционал                   | Поддерживается |
|:----------------------------------------------:|:--------------:|
|                Многопоточность                 |       ✔️       | 
|            Привязка прокси к сессии            |       ✔️       | 
| Авто-регистрация аккаунта по вашей реф. ссылке |       ✔️       |
|       Автоматическое улучшение бустеров        |       ✔️       |
|          Поддержка pyrogram .session           |       ✔️       |


## [Настройки](https://github.com/Cybertat1on/Qlyuker/blob/main/.env-example/)
|        Настройки         |                                                                                             Описание                                                                                              |
|:------------------------:|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
|  **API_ID / API_HASH**   |                                                        Данные платформы, с которой будет запущена сессия Telegram (по умолчанию - android)                                                        |
|        **REF_ID**        |                                                              Ваш реферальный аргумент (идет после app/startapp? в вашей реф. ссылке)                                                              |
|         **TAPS**         |                                                       Список значений, определяющий количество кликов за один цикл (по умолчанию [10, 100])                                                       |
|     **ENABLE_TAPS**      |                                                                    Включения/отключения функции «Тапов» (по умолчанию - True)                                                                     |
| **ENABLE_CLAIM_REWARDS** |                                                                 Включения/отключения функции «Сбор Наград» (по умолчанию - True)                                                                  |
|   **ENABLE_UPGRADES**    |                                                                  Включения/отключения функции «Апгрейдов» (по умолчанию - True)                                                                   |
|     **ENABLE_TASKS**     |                                                               Включения/отключения функции «Выполнения задач» (по умолчанию - True)                                                               |
|      **MAX_INCOME**      | Максимальный доход в час, после достижения которого прекращаются улучшения. Значение 0 означает отсутствие лимита. Пример: 1000000 остановит улучшения после достижения 1М/час (по умолчанию - 0) |
|   **MAX_LEVEL_PROMO**    |               Максимальный уровень карточек в пассивном доходе, после достижения которого прекращаются улучшения (по умолчанию - 10 уровень). Для всех карточек одинаковое значение               |
|   **MAX_LEVEL_ENERGY**   |                                             Максимальный уровень энергии, после достижения которого прекращаются улучшения (по умолчанию - 5 уровень)                                             |
|    **MAX_LEVEL_TAP**     |                                              Максимальный уровень клика, после достижения которого прекращаются улучшения (по умолчанию - 5 уровень)                                              |
| **SLEEP_AFTER_UPGRADE**  |                                                                     Время задержки после апгрейда (по умолчанию - 1 секунда)                                                                      |
| **SLEEP_ON_LOW_ENERGY**  |                                                         Время ожидания при низком уровне энергии.Значение в секундах (по умолчанию - 900)                                                         |
|  **SLEEP_BETWEEN_TAPS**  |                                                            Список значений, определяющий задержку между кликами (по умолчанию [1, 3])                                                             |
| **DELAY_BETWEEN_TASKS**  |                                                     Список значений, определяющий задержку между выполнением заданий(по умолчанию - [3, 15])                                                      |
|   **ENERGY_THRESHOLD**   |                                                                    Порог энергии для выполнения действий (по умолчанию - 0.05)                                                                    |
| **USE_PROXY_FROM_FILE**  |                                                              Использовать ли прокси из файла `bot/config/proxies.txt` (True / False)                                                              |

## Быстрый старт 📚

Для быстрой установки и последующего запуска - запустите файл `run.bat` на **Windows** или `run.sh` на **Линукс**

## Предварительные условия
Прежде чем начать, убедитесь, что у вас установлено следующее:
- [Python](https://www.python.org/downloads/release/python-3100/) **версии 3.11.5**


## Прокси
Перед началом удалить всё с файла `bot/config/proxies.txt`, потом вводите свои данные. Прокси можно отправлять в формате:
```text
type://user:pass@ip:port
type://user:pass:ip:port
type://ip:port:user:pass
type://ip:port@user:pass
type://ip:port
```
где:
```text
type - это тип прокси "http", "https", "socks4", "socks5"
```

## Получение API ключей
1. Перейдите на сайт [**my.telegram.org**](https://my.telegram.org/auth) и войдите в систему, используя свой номер телефона.
2. Выберите `API development tools` и заполните форму для регистрации нового приложения.
3. Запишите `API_ID` и `API_HASH` в файле `.env`, предоставленные после регистрации вашего приложения.

## Установка
Вы можете скачать [**Репозиторий**](https://github.com/Cybertat1on/Qlyuker) клонированием на вашу систему и установкой необходимых зависимостей:
```shell
git clone https://github.com/Cybertat1on/Qlyuker.git
cd Qlyuker
```

Затем для автоматической установки введите:

Windows:
```shell
run.bat
```

Linux:
```shell
run.sh
```

# Linux ручная установка
```shell
sudo sh install.sh
python3 -m venv venv
source venv/bin/activate
pip3 install -r requirements.txt
cp .env-example .env
nano .env  # Здесь вы обязательно должны указать ваши API_ID и API_HASH , остальное берется по умолчанию
python3 main.py
```

Также для быстрого запуска вы можете использовать аргументы, например:
```shell
~/Qlyuker >>> python3 main.py --action (1/2)
# Or
~/Qlyuker >>> python3 main.py -a (1/2)

# 1 - Запускает кликер
# 2 - Создает сессию
```


# Windows ручная установка
```shell
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
copy .env-example .env
# Указываете ваши API_ID и API_HASH, остальное берется по умолчанию
python main.py
```

Также для быстрого запуска вы можете использовать аргументы, например:
```shell
~/Qlyuker >>> python main.py --action (1/2)
# Или
~/Qlyuker >>> python main.py -a (1/2)

# 1 - Запускает кликер
# 2 - Создает сессию
```

