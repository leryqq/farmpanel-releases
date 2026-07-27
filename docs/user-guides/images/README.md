# Скриншоты для руководств

В этой папке хранятся изображения, на которые ссылаются гайды из `docs/user-guides/`.
Каждый гайд лежит в своей подпапке (`user-guide/`, `install-guide/`, `install-sandboxie-plus/`), поэтому в самих `.md` используются относительные ссылки вида `![подпись](../images/имя-файла.png)` (на один уровень вверх).

## Как добавить скриншот

1. Сделайте скриншот и сохраните его **точно под тем именем**, которое указано в списке ниже.
2. Положите файл в эту папку (`images/`), а скриншоты Sandboxie-Plus — в подпапку `images/sandboxie/`.
3. Готово — ссылка в гайде подхватит картинку автоматически.

## Соглашения

- **Формат:** PNG для скриншотов интерфейса.
- **Ширина:** 1280–1920 px. Размер файла желательно до ~300–500 КБ.
- **Имена:** латиница, `kebab-case`, без пробелов.
- **Один файл — на все языки.** RU/EN/ES-версии `USER-GUIDE` ссылаются на одни и те же файлы; переводится только подпись в тексте гайда, не имя файла.

## Список нужных файлов

Скриншоты, общие для `USER-GUIDE.ru.md` / `USER-GUIDE.md` / `USER-GUIDE.es.md`:

- [ ] `dashboard-overview.png` — главный экран (Dashboard), обзорный
- [ ] `setup-installer.png` — окно установщика Setup.exe
- [ ] `license-activation.png` — окно активации лицензии
- [ ] `window-layout.png` — общая структура окна с подписанными областями
- [ ] `command-palette.png` — открытая палитра команд (Ctrl+K)
- [ ] `sidebar.png` — боковая панель со всеми разделами
- [ ] `dashboard-screen.png` — Dashboard с полосой показателей и лентой событий
- [ ] `accounts-screen.png` — экран Accounts с таблицей и панелью сведений
- [ ] `workflows-screen.png` — экран Workflows (три панели)
- [ ] `matchmaking-screen.png` — экран Matchmaking (группы и подробности)
- [ ] `monitoring-screen.png` — экран Monitoring (датчики и список процессов)
- [ ] `logs-screen.png` — экран Logs (журнал событий)
- [ ] `layouts-screen.png` — экран Layouts (холст мониторов)
- [ ] `settings-screen.png` — экран Settings
- [ ] `accounts-add-form.png` — форма добавления аккаунта
- [ ] `import-wizard-validation.png` — мастер импорта, шаг проверки строк
- [ ] `accounts-bulk-start.png` — массовый запуск, статусы Starting/Running
- [ ] `matchmaking-party-queue.png` — группа в очереди с позициями участников
- [ ] `matchmaking-match-found.png` — плашка Match Found
- [ ] `status-recovering.png` — значок Recovering в строке состояния
- [ ] `status-badges.png` — примеры статусов в таблице аккаунтов
- [ ] `notification-error-toast.png` — всплывающее уведомление об ошибке (View / Retry)
- [ ] `error-screen.png` — экран с ошибкой (Retry / Open logs)

Скриншоты для `INSTALL-GUIDE.ru.md`:

- [ ] `install-download-page.png` — страница загрузки с файлом Setup.exe
- [ ] `initial-setup-locations.png` — первичная настройка: расположение Steam и Sandboxie
- [ ] `license-activation.png` — *(тот же файл, что и в USER-GUIDE)*
- [ ] `dashboard-overview.png` — *(тот же файл, что и в USER-GUIDE)*

Скриншоты для `INSTALL-SANDBOXIE-PLUS.ru.md` (папка `sandboxie/`):

- [x] `sandboxie/github-release-assets.png` — страница релиза 1.17.5 с разделом Assets
- [x] `sandboxie/installer-wizard.png` — экран мастера установки с папкой по умолчанию
- [x] `sandboxie/main-window.png` — главное окно Sandboxie-Plus после первого запуска

Экраны мастера первичной настройки (Setup Wizard), Шаг 4 — по одному на этап:

- [x] `sandboxie/wizard-1-introduction.png` — экран 1, Introduction («Personally, for private non-commercial use»)
- [x] `sandboxie/wizard-2-support-certificate.png` — экран 2, Support certificate (поле пустое)
- [x] `sandboxie/wizard-3-ui-configuration.png` — экран 3, Configure UI (значения по умолчанию)
- [x] `sandboxie/wizard-4-shell-integration.png` — экран 4, Shell integration (галочки сняты)
- [x] `sandboxie/wizard-5-updater.png` — экран 5, Updater (галочки сняты)
- [x] `sandboxie/wizard-6-complete.png` — экран 6, Complete (кнопка Finish)
