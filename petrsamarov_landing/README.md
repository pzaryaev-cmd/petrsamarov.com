# petrsamarov.com landing

Внутри готовый статический сайт для Vercel.

## Что уже добавлено

1. Open Graph и Twitter Card: при отправке ссылки в Telegram/соцсети должна появляться карточка с изображением `assets/og-image.png`.
2. Favicon: значки вкладки браузера лежат в `assets/`.
3. Vercel Web Analytics: скрипт уже добавлен в `index.html`, но аналитику нужно включить в Vercel Dashboard.
4. SEO-база: canonical, robots.txt, sitemap.xml, description.
5. Блок «Об авторе» ожидает файл `assets/author.jpg`. Если его нет, сайт автоматически покажет символ Предела.

## Как обновить сайт на Vercel

Загрузи всю папку `petrsamarov_landing` заново как проект или обнови текущий проект тем же способом, которым загружал первую версию.

Важно: в корне должны лежать:

- `index.html`
- `assets/`
- `robots.txt`
- `sitemap.xml`
- `site.webmanifest`

## Google Analytics 4

В `index.html` есть закомментированный блок Google Analytics.
Когда создашь GA4 Measurement ID вида `G-XXXXXXXXXX`, замени оба `G-XXXXXXXXXX` на свой ID и убери HTML-комментарий вокруг блока.

## Vercel Analytics

В Vercel Dashboard открой проект → Analytics → Enable Web Analytics.
Скрипт уже добавлен:

```html
<script defer src="/_vercel/insights/script.js"></script>
```
