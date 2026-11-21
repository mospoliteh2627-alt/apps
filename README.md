# Сборки приложений — страница скачивания

Три Android-приложения, готовые к установке: FinBridge, «Вектор Банк» (магистерский прототип), CraftLearn.

## Что внутри

| Файл | Приложение | Пакет | Версия | Размер |
|---|---|---|---|---|
| `files/FinBridge-1.0.0.apk` | FinBridge | `ru.finbridge.finbridge` | 1.0.0 | 49 МБ |
| `files/VectorBank-1.0.0.apk` | Вектор Банк | `com.vectorbank.vector_bank_mobile` | 1.0.0 | 64 МБ |
| `files/CraftLearn-1.0.0.apk` | CraftLearn | `ru.craftlearn.app` | 1.0 | 1 МБ |

`index.html` — страница скачивания, `img/` — иконки и скриншоты.

## Подписи

- `VectorBank`, `CraftLearn` пересобраны на релизном ключе `.keys/dsh-release.jks` (alias `dsh-release`, пароль в `.keys/keystore.properties`). Ключ хранится в воркспейсе — обновления подписывать только им.
- `FinBridge` сохранён с проектным ключом `CN=FinBridge` (`projects/mospolytech/7845`), чтобы совпадать с будущими сборками из исходников.
- Debug-подписи заменены: если на телефоне стояла прежняя debug-сборка, её нужно удалить перед установкой.

## Публикация

Вариант 1 — GitHub Pages: залить папку в публичный репозиторий, включить Pages, ссылка `https://<user>.github.io/<repo>/`.

Вариант 2 — GitHub Releases: приложить APK к релизу, в `index.html` заменить `files/…` на `https://github.com/<user>/<repo>/releases/latest/download/<файл>.apk` — тогда страницу можно держать где угодно.

Вариант 3 — свой домен: положить папку на хостинг, например `https://guvanch.ru/apps/`.
