# Plazma Sign Bridge — готовые сборки

Публичный канал подписанных сборок расширения для Chromium-браузеров на Windows.
Исходников серверной части в этом репозитории нет. Вход в GitHub для скачивания не требуется.

## Проверка обновления 0.2.0 → 0.2.1

1. Оставьте установленное расширение на версии **0.2.0**.
2. Скачайте [только помощника версии 2](https://github.com/plazma-devhub/plazma-sign-bridge-releases/releases/download/extension-v0.2.1/plazma-sign-bridge-updater-windows.zip).
3. Полностью распакуйте ZIP и запустите `Install-Updater.cmd`.
4. Выберите прежнюю папку расширения и укажите его ID со страницы `chrome://extensions` (Edge: `edge://extensions`). Запрос предыдущего ID пропустите клавишей Enter.
5. Перезагрузите расширение. Нажмите **«Проверить обновления» → «Обновить»**.
6. Убедитесь, что появилась версия **0.2.1**, а ID и настройки сохранились. Обновите рабочие вкладки.
7. Для проверки возврата нажмите **«Откатить»** — вернётся 0.2.0.

Папку расширения вручную заменять на 0.2.1 для этого теста не нужно.
Автоматическое обновление требует отдельной рабочей папки вне Git checkout.

## Новая установка

[Полный комплект Windows](https://github.com/plazma-devhub/plazma-sign-bridge-releases/releases/download/extension-v0.2.1/plazma-sign-bridge-windows.zip) содержит расширение и помощника.
Распакуйте его в постоянную папку, загрузите подпапку `bnovo-sign-bridge` как распакованное расширение в режиме разработчика браузера и запустите установщик помощника.

[Все релизы](https://github.com/plazma-devhub/plazma-sign-bridge-releases/releases).

## Канал обновлений

Подписанное описание: [update.json](https://github.com/plazma-devhub/plazma-sign-bridge-releases/releases/download/extension-latest/update.json).
Помощник проверяет RSA-подпись и контрольные суммы перед применением. Закрытого ключа подписи, паролей и GitHub-токенов в комплекте нет.
