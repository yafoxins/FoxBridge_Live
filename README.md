# <div align="center"><img src="foxbridge-app/src-tauri/icons/128x128.png" width="128" alt="FoxBridge Live logo" /></div>

# <div align="center">FoxBridge Live</div>

<p align="center">
  <b>Профессиональное связующее звено между вашей аудиторией в VK Live и миром VTube Studio.</b><br />
  Автоматизируйте взаимодействие со зрителями и превратите каждый подарок в живую эмоцию вашего аватара.
</p>

<p align="center">
  <a href="https://vtubing.ru">
    <img src="https://img.shields.io/badge/Сайт-vtubing.ru-7C5CFF?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Website" />
  </a>
  <a href="https://github.com/yafoxins/FoxBridge_Live/releases">
    <img src="https://img.shields.io/badge/Скачать-Releases-EA4AAA?style=for-the-badge" alt="Releases" />
  </a>
  <a href="https://t.me/yafoxindev">
    <img src="https://img.shields.io/badge/Telegram-Сообщество-2AABEE?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram" />
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/OS-Windows-0078D6?style=flat-square&logo=windows&logoColor=white" alt="Windows" />
  <img src="https://img.shields.io/badge/Backend-Rust_%7C_Tauri-24C8DB?style=flat-square&logo=rust&logoColor=white" alt="Rust" />
  <img src="https://img.shields.io/badge/Frontend-React_%7C_TypeScript-3178C6?style=flat-square&logo=react&logoColor=white" alt="React" />
  <img src="https://img.shields.io/badge/Database-SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white" alt="SQLite" />
</p>

---

## 🛠 Как это работает?

```mermaid
graph LR
    A[👤 Зритель в VK Live] -- Дарит награду --> B(🌐 FoxBridge Bridge)
    B -- Передает событие --> C{🦊 FoxBridge Live}
    C -- Проверяет привязку --> D[⌨️ VTube Studio Hotkey]
    D -- Запускает анимацию --> E[💃 Ваш 2D Аватар]
    
    style C fill:#f96,stroke:#333,stroke-width:2px
    style E fill:#bbf,stroke:#333,stroke-width:2px
```

---

## ✨ Ключевые преимущества

### 🧠 Интеллектуальная обработка (FIFO)
Больше никакой путаницы и пропущенных наград. Система **Smart Queue** гарантирует, что все события будут выполнены по очереди. Каждая награда имеет свой независимый «поток», поэтому кулдаун одного триггера никогда не заблокирует выполнение других.

### 🔌 Бесшовная интеграция
FoxBridge Live автоматически обнаруживает запущенную **VTube Studio** и подключается к ней по локальному API. Список ваших хоткеев подгружается мгновенно — вам остается только выбрать нужный.

### 🛡 Безопасность прежде всего
*   **Локальное хранение**: Ваши данные и настройки хранятся только на вашем компьютере.
*   **Relay-авторизация**: Мы используем защищенный механизм передачи событий, чтобы ваши токены VK никогда не подвергались риску.

### 💎 Премиальный UX
*   **Сворачивание в трей**: Приложение работает тихо в фоне, не отвлекая от процесса стрима.
*   **Живой лог**: Наблюдайте за обработкой наград в реальном времени с детальной историей.
*   **Автоподключение**: Настройте один раз — и приложение будет само восстанавливать связь с VTS при каждом запуске.

---

## 🚀 Быстрый старт

1.  **Установка**: Скачайте и запустите установщик со страницы [Releases](https://github.com/yafoxins/FoxBridge_Live/releases).
2.  **VTube Studio**: Включите "Start API" в настройках (раздел Plugins).
3.  **Связь**: Войдите через VK и создайте привязки во вкладке "Триггеры".
4.  **Готово**: Наслаждайтесь новым уровнем взаимодействия с аудиторией!

---

## 👥 Команда проекта

| Роль | Профиль | Контакты |
| :--- | :--- | :--- |
| **Разработчик** | **YaFoxin Dev** | [![TG](https://img.shields.io/badge/-Telegram-2AABEE?style=flat-square&logo=telegram&logoColor=white)](https://t.me/yafoxindev) [![GH](https://img.shields.io/badge/-GitHub-171515?style=flat-square&logo=github&logoColor=white)](https://github.com/yafoxins) |
| **Вдохновитель** | **Naynoira** | [![Twitch](https://img.shields.io/badge/-Twitch-9146FF?style=flat-square&logo=twitch&logoColor=white)](https://www.twitch.tv/naynoira) [![TG](https://img.shields.io/badge/-Telegram-2AABEE?style=flat-square&logo=telegram&logoColor=white)](https://t.me/naynoira) |

---

## 🤝 Поддержка и обратная связь

Мы активно развиваем проект и прислушиваемся к сообществу.
*   🌐 Официальный портал: [vtubing.ru](https://vtubing.ru)
*   🐛 Нашли ошибку? [Создайте Issue](https://github.com/yafoxins/FoxBridge_Live/issues)
*   📢 Новости и обновления в нашем [Telegram-канале](https://t.me/yafoxindev)

---

## 📄 Лицензия

Проект распространяется под лицензией **MIT**. Полный текст в файле [LICENSE](LICENSE).

<p align="center">
  <i>Сделано с ❤️ для стримеров нового поколения.</i>
</p>
