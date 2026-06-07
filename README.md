# GoTelegram: Безопасный MTProxy с Fake TLS

Ультимативное решение для стабилизации работы Telegram. Скрипт маскирует трафик под обычные сайты, работает через Docker с автозапуском и управляется одной короткой командой.

---

## Особенности
* **Маскировка (Fake TLS):** Провайдер видит, что вы просто читаете новости или Википедию. Трафик не определяется как прокси.
* **Быстрый выбор:** Список из предустановленных популярных доменов или ввод своего.
* **Автоматизация:** Полная настройка Docker и зависимостей "под ключ" за один запуск.
* **Удобное управление:** Команда `gotelegram` доступна в консоли сразу после установки.
* **QR-коды:** Генерация рабочих QR-кодов прямо в терминале для мгновенного подключения с телефона.

---

## Быстрая установка на сервере

Через терминал (Ubuntu/Debian/CentOS):

```bash
wget -O setup_gotelegram.sh https://raw.githubusercontent.com/swr8bit/mtproxy_gotelegram/main/setup_gotelegram.sh && chmod +x setup_gotelegram.sh && sudo ./setup_gotelegram.sh
```
#### Запуск
```bash
gotelegram
```

### Если вы не root
```bash
sudo -i bash -c "wget -O setup_gotelegram.sh https://raw.githubusercontent.com/swr8bit/mtproxy_gotelegram/main/setup_gotelegram.sh && chmod +x setup_gotelegram.sh && ./setup_gotelegram.sh"
```

#### Запуск
```bash
sudo gotelegram
```
---

## Зависимости

Этот скрипт использует готовый Docker-образ от разработчика **Sergey Arkhipov** (9seconds).

- **Источник образа:** Docker Hub (`nineseconds/mtg:2`)
- **Репозиторий исходного кода:** [https://github.com/9seconds/mtg](https://github.com/9seconds/mtg)
- **Лицензия:** MIT

Все права на код mtg принадлежат Sergey Arkhipov.

## Важное уведомление об авторских правах
Данный проект включает в себя исходный код, созданный пользователем anten-ka (https://github.com/anten-ka). Этот код не содержит явной лицензии на использование. В соответствии с действующим законодательством об авторском праве, все права на оригинальный код принадлежат его создателю.

Мои собственные изменения и дополнения к этому коду распространяются под лицензией MIT. Полный текст лицензии доступен в файле LICENSE
