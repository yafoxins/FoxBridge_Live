# <div align="center"><img src="foxbridge-app/src-tauri/icons/128x128.png" width="96" alt="FoxBridge Live logo" /></div>

# <div align="center">FoxBridge Live</div>

<p align="center">
  <b>Ультимативный мост между вашими зрителями в VK Live и магией VTube Studio.</b><br />
  Оживите своего аватара с помощью интерактивных наград, работающих без задержек и сбоев.
</p>

<p align="center">
  <a href="https://vtubing.ru">
    <img src="https://img.shields.io/badge/Сайт-vtubing.ru-7C5CFF?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Website" />
  </a>
  <a href="https://github.com/yafoxins/FoxBridge_Live/releases">
    <img src="https://img.shields.io/badge/Скачать-v0.3.4-EA4AAA?style=for-the-badge" alt="Releases" />
  </a>
  <a href="https://t.me/yafoxindev">
    <img src="https://img.shields.io/badge/Telegram-Канал-2AABEE?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram" />
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Windows-10%20%2F%2011-0078D6?style=flat-square&logo=windows&logoColor=white" alt="Windows 10/11" />
  <img src="https://img.shields.io/badge/VK%20Live-Интеграция-2787F5?style=flat-square" alt="VK Live" />
  <img src="https://img.shields.io/badge/Tauri-2.x-24C8DB?style=flat-square&logo=tauri&logoColor=white" alt="Tauri 2" />
  <img src="https://img.shields.io/badge/Rust-Core-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust" />
</p>

---

## ✨ Что нового в v0.3.4?

Мы полностью переработали внутреннюю логику приложения, чтобы сделать его самым стабильным инструментом для стримеров на рынке.

### 🧠 Умная очередь (FIFO) и Smart Cooldown
Больше никаких «пропущенных» наград из-за того, что предыдущая еще не закончилась.
*   **Параллельные линии**: Кулдаун одной награды больше не блокирует выполнение других. Каждая награда теперь имеет свой независимый «поток».
*   **Очередь без потерь**: Если вам прислали 10 одинаковых наград подряд, FoxBridge Live аккуратно выстроит их в очередь и выполнит одну за другой, соблюдая заданные паузы.
*   **Интеллектуальное ожидание**: В журнале наглядно отображается статус «Ожидание кулдауна», если зрители засыпали вас подарками.

### 🛡 Безопасность и Архитектура
*   **Relay-авторизация**: Ваши токены VK остаются в безопасности и никогда не покидают ваше устройство в открытом виде.
*   **Новая схема БД**: Мы перешли на гибкую структуру SQLite, что решило проблемы с авторизацией и синхронизацией каналов.
*   **Автономность**: Приложение корректно инициализирует сессии при первом запуске, исключая ошибки подключения.

### 💎 Дизайн и UX (User Experience)
*   **Живой Журнал событий**: История наград теперь обновляется автоматически каждые 2 секунды. Вам не нужно кликать по вкладкам, чтобы увидеть свежее событие.
*   **Полный контроль**: Добавлены кнопки **Удалить** (очистка истории) и **Отменить** (ручной пропуск активного события) для каждой записи.
*   **Настоящий Трей**: Теперь приложение действительно сворачивается в системный лоток и работает в фоне. Открытие окна доступно по клику на иконку в трее.
*   **VTS Auto-connect**: Приложение само находит VTube Studio и подключается к ней, запоминая ваш порт (даже если он отличен от 8001).

---

## 📺 Демонстрация работы

[![Смотреть демонстрацию FoxBridge Live на YouTube](https://img.youtube.com/vi/rmEiSecHBsc/maxresdefault.jpg)](https://www.youtube.com/watch?v=rmEiSecHBsc)

---

## 🚀 Как начать работу

1.  **Скачайте** актуальную версию со страницы [Releases](https://github.com/yafoxins/FoxBridge_Live/releases).
2.  **Запустите VTube Studio** и включите "Start API" в настройках плагинов.
3.  **Авторизуйтесь** через VK в приложении FoxBridge Live.
4.  Создайте привязки на вкладке **Триггеры**.
5.  **Готово!** Окунитесь в интерактив со своими зрителями.

---

## 🛠 Технологический стек

*   **Rust (Tauri 2)** — максимальная производительность и минимальное потребление ОЗУ.
*   **React 18 + Vite** — быстрый и плавный интерфейс.
*   **Tailwind CSS + Framer Motion** — современный дизайн с мягкими анимациями.
*   **SQLite** — надежное локальное хранилище данных.

---

## 🤝 Поддержка и обратная связь

Если у вас есть идеи по улучшению или вы нашли ошибку:
*   🌐 Наш сайт: [vtubing.ru](https://vtubing.ru)
*   📢 Telegram: [@yafoxindev](https://t.me/yafoxindev)
*   🐛 GitHub Issues: [Открыть тикет](https://github.com/yafoxins/FoxBridge_Live/issues)

---

## 📄 Лицензия

Распространяется под лицензией **MIT**. Подробности в файле [LICENSE](LICENSE).

<p align="center">
  Разработано с ❤️ командой <b>YaFoxin | Dev</b> и вдохновлено <b>Naynoira</b>.
</p>
