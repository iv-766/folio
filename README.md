# Igor Veshutkin — Portfolio

Статичный сайт-портфолио. Для публикации на GitHub Pages:

1. Создать репозиторий и залить содержимое этой папки в корень (index.html должен лежать в корне ветки).
2. Settings → Pages → Source: **Deploy from a branch**, ветка `main`, папка `/ (root)`.
3. Сайт будет доступен по адресу `https://<username>.github.io/<repo>/`.

Файл `.nojekyll` нужен, чтобы GitHub не обрабатывал папки Jekyll-ом — не удалять.

## Структура
- `index.html` — весь сайт
- `support.js` — рантайм, обязателен рядом с index.html
- `assets/` — изображения кейсов, портрет, CV
- `audio/` — треки плеера
