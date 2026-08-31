# Igor Veshutkin — Portfolio

Статичный сайт-портфолио. Для публикации на GitHub Pages:

1. Создать репозиторий и залить содержимое этой папки в корень (index.html должен лежать в корне ветки).
2. Settings → Pages → Source: **Deploy from a branch**, ветка `main`, папка `/ (root)`.
3. Сайт будет доступен по адресу `https://<username>.github.io/<repo>/`.

Файл `.nojekyll` нужен, чтобы GitHub не обрабатывал папки Jekyll-ом — не удалять.

## Структура
- `index.html` — весь сайт
- `support.js` — рантайм, обязателен рядом с index.html
- `assets/` — изображения кейсов, портрет, CV (PDF), `assets/research/` — исследования и UX-карты
- `audio/` — треки плеера

## Кэш
В `index.html` стоят мета-теги `no-cache` и версия сборки (`build-version`), а `support.js` подключается с `?v=<версия>`.

При каждом обновлении сайта меняй версию в двух местах `index.html`:
- `<meta name="build-version" content="ГГГГММДД">`
- `<script src="./support.js?v=ГГГГММДД">`

Если менялись картинки под теми же именами — добавь `?v=ГГГГММДД` и к ним. Тогда посетителям не нужно сбрасывать кэш.
