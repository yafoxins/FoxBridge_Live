# <div align="center"><img src="src-tauri/icons/128x128.png" width="96" alt="FoxBridge Live logo" /></div>

# <div align="center">FoxBridge Live</div>

<p align="center">
  Desktop-приложение для Windows, которое связывает награды <b>VK Live</b> с hotkeys в <b>VTube Studio</b>.
</p>

<p align="center">
  <a href="https://github.com/yafoxins/FoxBridge_Live/releases">
    <img src="https://img.shields.io/badge/Скачать-Releases-EA4AAA?style=for-the-badge" alt="Releases" />
  </a>
  <a href="https://t.me/yafoxindev">
    <img src="https://img.shields.io/badge/Telegram-YaFoxin_Dev-2AABEE?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram" />
  </a>
  <a href="https://github.com/yafoxins/FoxBridge_Live">
    <img src="https://img.shields.io/badge/GitHub-FoxBridge__Live-171515?style=for-the-badge&logo=github&logoColor=white" alt="GitHub repository" />
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Windows-10%20%2F%2011-0078D6?style=flat-square&logo=windows&logoColor=white" alt="Windows 10/11" />
  <img src="https://img.shields.io/badge/VK%20Live-Награды%20и%20события-2787F5?style=flat-square" alt="VK Live" />
  <img src="https://img.shields.io/badge/VTube%20Studio-Hotkeys%20API-7C5CFF?style=flat-square" alt="VTube Studio" />
  <img src="https://img.shields.io/badge/Tauri-2.x-24C8DB?style=flat-square&logo=tauri&logoColor=white" alt="Tauri 2" />
  <img src="https://img.shields.io/badge/React-18-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="React 18" />
  <img src="https://img.shields.io/badge/TypeScript-5.x-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript 5" />
  <img src="https://img.shields.io/badge/Rust-Desktop%20Core-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust" />
  <img src="https://img.shields.io/badge/SQLite-Local%20Storage-003B57?style=flat-square&logo=sqlite&logoColor=white" alt="SQLite" />
</p>

## Что это

**FoxBridge Live** нужен для простого сценария:

1. зритель активирует награду в **VK Live**
2. приложение получает событие
3. находит нужную привязку
4. отправляет hotkey в **VTube Studio**
5. модель реагирует автоматически

Без ручной рутины, без сложной сервисной настройки и без постоянного переключения между разными окнами.

## Почему FoxBridge Live

- **Простой старт**. Пользователю не нужно вручную разбираться с webhook URL, redirect URL и служебными настройками API.
- **Фокус на стриме**. В интерфейсе остаются только действительно нужные вещи: вход, канал, триггеры и журнал.
- **Быстрая реакция модели**. Награды VK Live можно привязать к hotkeys VTube Studio и получать понятный результат сразу.
- **Нормальный UX для Windows**. Это не набор скриптов, а полноценное desktop-приложение с установщиком.
- **Локальное хранение настроек**. Канал, привязки, токены и история действий сохраняются между перезапусками.

## Что умеет

- вход через **VK Live**
- выбор и сохранение канала
- получение событий наград
- автоматическая синхронизация наград после авторизации
- подключение к **VTube Studio** по локальному API
- загрузка и сохранение списка hotkeys
- привязка наград к hotkeys
- поддержка cooldown между срабатываниями
- журнал последних событий и результатов

## На чём написан проект

FoxBridge Live собран как desktop-приложение на современном стеке:

- **Tauri 2 + Rust** для нативной Windows-части, системной логики и локального хранения
- **React 18 + TypeScript + Vite** для интерфейса
- **Zustand** для клиентского состояния
- **Tailwind CSS + Framer Motion** для интерфейса и анимаций
- **SQLite** для локальной базы приложения
- **NSIS** для Windows-установщика

## Для кого подходит

FoxBridge Live подойдёт, если вы:

- стримите через **VK Live**
- используете **VTube Studio**
- хотите быстро связать награды канала с реакциями модели
- не хотите вручную собирать служебную инфраструктуру вокруг интеграции

## Как начать

1. Скачайте актуальный установщик из раздела [Releases](https://github.com/yafoxins/FoxBridge_Live/releases).
2. Установите **FoxBridge Live** на Windows.
3. Запустите приложение и войдите через **VK Live**.
4. Подключите **VTube Studio**.
5. На экране `Триггеры` создайте привязки между наградами и hotkeys.
6. Проверьте результат в журнале событий.

## FAQ

<details>
  <summary><b>Почему исходный код не опубликован?</b></summary>
  <br />
  Этот репозиторий используется как публичная витрина приложения, место для установщиков, релизов и пользовательской информации. Исходный код проекта в открытом виде не распространяется.
</details>

<details>
  <summary><b>Нужно ли мне самому настраивать VK API?</b></summary>
  <br />
  В обычном пользовательском сценарии нет. Приложение рассчитано так, чтобы в интерфейсе оставались только вход, канал, триггеры и журнал.
</details>

<details>
  <summary><b>Подходит ли приложение только для VTuber-стримов?</b></summary>
  <br />
  В первую очередь да: FoxBridge Live создавался именно для связки наград VK Live с реакциями модели в VTube Studio. Но его можно использовать и в любых похожих интерактивных сценариях, где нужен запуск hotkeys по событию.
</details>

<details>
  <summary><b>Какая ОС поддерживается?</b></summary>
  <br />
  На текущий момент основной сценарий рассчитан на <b>Windows 10 / 11</b>.
</details>

<details>
  <summary><b>Что нужно для работы кроме приложения?</b></summary>
  <br />
  Нужны установленный <b>VTube Studio</b>, рабочий аккаунт <b>VK Live</b> и доступ к локальному API VTube Studio, обычно через <code>127.0.0.1:8001</code>.
</details>

## Скачать

- Репозиторий: [github.com/yafoxins/FoxBridge_Live](https://github.com/yafoxins/FoxBridge_Live)
- Релизы и установщики: [github.com/yafoxins/FoxBridge_Live/releases](https://github.com/yafoxins/FoxBridge_Live/releases)

## Автор

**YaFoxin Dev**

- Telegram: [t.me/yafoxindev](https://t.me/yafoxindev)
- GitHub: [github.com/yafoxins](https://github.com/yafoxins)

## Обратная связь

Если вы нашли баг, хотите предложить улучшение или нужна помощь по приложению, можно:

- написать в Telegram: [t.me/yafoxindev](https://t.me/yafoxindev)
- открыть issue в репозитории: [github.com/yafoxins/FoxBridge_Live/issues](https://github.com/yafoxins/FoxBridge_Live/issues)
