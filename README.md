# Портал Легенд — music hub

Одностраничный сайт-хаб с биографиями, дискографиями и ссылками на стриминги.

## Состав архива

- `music-hub.html` — весь сайт
- `bg.gif` — фоновая гифка (лежит рядом с html)
- `covers/` — обложки альбомов (Marilyn Manson и др.)
- `README.md` — этот гайд

## Как открыть локально

1. Распакуй zip в любую папку.
2. Открой `music-hub.html` в браузере (Chrome / Firefox / Edge).
3. Важно: `bg.gif` и папка `covers` должны лежать **в той же папке**, что и html.

---

## Выгрузка на GitHub Pages

1. Зайди на [github.com](https://github.com) → **New repository**.
2. Название, например: `portal-legend` → Create (можно **Public**).
3. На странице репозитория: **Add file → Upload files**.
4. Перетащи сюда:
   - `music-hub.html`
   - `bg.gif`
   - папку `covers` (все файлы внутри)
5. Commit changes.
6. **Settings → Pages** (слева).
7. Source: **Deploy from a branch** → Branch: `main` (или `master`) → folder **/ (root)** → Save.
8. Через 1–2 минуты сайт будет по адресу:
   `https://ТВОЙ_НИК.github.io/portal-legend/music-hub.html`  
   (или переименуй html в `index.html` — тогда откроется сразу корень).

### Чтобы открывался с корня

Переименуй `music-hub.html` → `index.html` перед загрузкой (или после, через GitHub web editor).

---

## Выгрузка на grok.mi (и похожие хостинги)

**grok.mi** — если это твой/другой статический хостинг с загрузкой файлов:

1. Зайди в панель хостинга / файловый менеджер.
2. Залей в **public_html** (или корень сайта):
   - `index.html` (переименуй music-hub.html)
   - `bg.gif`
   - папку `covers/`
3. Открой свой домен — сайт должен подхватить `index.html` сам.

Если grok.mi даёт только одну html-страницу без папок:

- либо залей zip и распакуй на сервере,
- либо в html временно убери зависимость от `covers/` (градиенты и так работают), а `bg.gif` положи рядом.

### Альтернативы бесплатно

- **GitHub Pages** — лучше всего для такого проекта.
- **Netlify Drop**: [app.netlify.com/drop](https://app.netlify.com/drop) — перетащи папку целиком.
- **Cloudflare Pages** / **Vercel** — через GitHub-репозиторий.

---

## Обложки

Сейчас локальные обложки подключены для **Marilyn Manson** (папка `covers/`).  
Остальные релизы — градиентные карточки + название.  
Чтобы добавить свою обложку:

1. Положи jpg/png в `covers/my-album.jpg`
2. В массиве альбомов у объекта добавь: `cover:'covers/my-album.jpg'`

---

## Сделано

alones_ с помощью Claude и Grok, 2026.
