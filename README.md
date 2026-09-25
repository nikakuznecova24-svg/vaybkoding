# vaybkoding
сайт услуг вайб-кодинга

## стили (важно!)

`assets/styles.css` — это заранее собранный Tailwind v4, а не CDN/на лету.
Если меняешь/добавляешь классы Tailwind в index.html, privacy.html или
quiz.html — новые классы не заработают, пока не пересобрать стили:

```
bun install
bun run build:css
```

После пересборки подними `?v=` у `<link rel="stylesheet" href="assets/styles.css?v=N">`
в index.html, чтобы сбросить кэш браузера/CDN.
