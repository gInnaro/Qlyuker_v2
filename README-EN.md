[![Static Badge](https://img.shields.io/badge/Telegram-Bot%20Link-Link?style=for-the-badge&logo=Telegram&logoColor=white&logoSize=auto&color=blue)](https://t.me/qlyukerbot/start?startapp=bro-1197825376)
[![Static Badge](https://img.shields.io/badge/Telegram-Channel-Link?style=for-the-badge&logo=Telegram&logoColor=white&logoSize=auto&color=blue)](https://t.me/CyberToolz)


#  Bot for Qlyuker


# 🔥🔥 PYTHON version must be 3.10 - 3.11.5 🔥🔥

> README на русском языке доступно [здесь](README.md)

## Features
|                    Feature                    |   Supported    |
|:---------------------------------------------:|:--------------:|
|                Multithreading                 |       ✔️       |
|         Proxy binding to the session          |       ✔️       |
| Auto-registration of the account via ref link |       ✔️      |  
|          Automatic booster upgrades           |       ✔️       |
|        Pyrogram .session file support         |       ✔️       |


## [Settings](https://github.com/Cybertat1on/Qlyuker/blob/main/.env-example/)
|         Setting          |                                                                  Description                                                                   |
|:------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------:|
|  **API_ID / API_HASH**   |                           Data of the platform from which the Telegram session will be launched (default - android)                            |
|        **REF_ID**        |                                    Your referral argument (comes after app/startapp? in your referral link)                                    |
|         **TAPS**         |                                   List of values defining the number of clicks per cycle (default [10, 100])                                   |
|     **ENABLE_TAPS**      |                                              Enable/disable the «Taps» function (default - True)                                               |
| **ENABLE_CLAIM_REWARDS** |                                         Enable/disable the «Collect Rewards» function (default - True)                                         |
|   **ENABLE_UPGRADES**    |                                            Enable/disable the «Upgrades» function (default - True)                                             |
|     **ENABLE_TASKS**     |                                          Enable/disable the «Task Launcher» feature (default – True)                                           |
|      **MAX_INCOME**      | Maximum income per hour limit after which upgrades stop. Value of 0 means no limit. Example: 1000000 will stop upgrades after reaching 1M/hour |
|   **MAX_LEVEL_PROMO**    |          Maximum level of cards in passive income after which improvements stop (default is level 10). All cards have the same value           |
|   **MAX_LEVEL_ENERGY**   |                                    Maximum energy level after which improvements stop (default is level 5)                                     |
|    **MAX_LEVEL_TAP**     |                                     Maximum click level, after which improvements stop (default - level 5)                                     |
| **SLEEP_AFTER_UPGRADE**  |                                                 Delay time after upgrade (default - 1 second)                                                  |
| **SLEEP_ON_LOW_ENERGY**  |                                          Timeout at low energy level.Value in seconds (default - 900)                                          |
|  **SLEEP_BETWEEN_TAPS**  |                                       List of values defining the delay between clicks (default [1, 3])                                        |
| **DELAY_BETWEEN_TASKS**  |                                      List of values defining the delay between tasks (default - [3, 15])                                       |
|   **ENERGY_THRESHOLD**   |                                            Energy threshold for performing actions (default - 0.05)                                            |
| **USE_PROXY_FROM_FILE**  |                                  Whether to use a proxy from the `bot/config/proxies.txt` file (True / False)                                  |


## Quick Start 📚

To fast install libraries and run bot - open `run.bat` on **Windows** or `run.sh` on **Linux**

## Prerequisites
Before you begin, make sure you have the following installed:
- [**Python**](https://www.python.org/downloads/release/python-3100/) **version 3.10**

## Proxies
Before you start, delete everything from the `bot/config/proxies.txt` file, then enter your data. Proxies can be sent in the format:
```text
type://user:pass@ip:port
type://user:pass:ip:port
type://ip:port:user:pass
type://ip:port@user:pass
type://ip:port
```
where:
```text
type is the proxy type “http”, “https”, “socks4”, “socks5”.
```

## Obtaining API Keys
1. Go to [**my.telegram.org**](https://my.telegram.org/auth) and log in using your phone number.
2. Select `API development tools` and fill out the form to register a new application.
3. Record the `API_ID` and `API_HASH` provided after registering your application in the `.env` file.

## Installation
You can download the [**repository**](https://github.com/Cybertat1on/Qlyuker) by cloning it to your system and installing the necessary dependencies:
```shell
git clone https://github.com/Cybertat1on/Qlyuker.git
cd Qlyuker
```

Then you can do automatic installation by typing:

Windows:
```shell
run.bat
```

Linux:
```shell
run.sh
```

# Linux manual installation
```shell
sudo sh install.sh
python3 -m venv venv
source venv/bin/activate
pip3 install -r requirements.txt
cp .env-example .env
nano .env  # Here you must specify your API_ID and API_HASH, the rest is taken by default
python3 main.py
```

You can also use arguments for quick start, for example:
```shell
~/Qlyuker >>> python3 main.py --action (1/2)
# Or
~/Qlyuker >>> python3 main.py -a (1/2)

# 1 - Run clicker
# 2 - Creates a session
```

# Windows manual installation
```shell
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
copy .env-example .env
# Here you must specify your API_ID and API_HASH, the rest is taken by default
python main.py
```

You can also use arguments for quick start, for example:
```shell
~/Qlyuker >>> python main.py --action (1/2)
# Or
~/Qlyuker >>> python main.py -a (1/2)

# 1 - Run clicker
# 2 - Creates a session
```
