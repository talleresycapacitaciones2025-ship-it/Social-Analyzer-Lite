# 🔎 Social Analyzer Lite

**Búsqueda de nombre de usuario en más de 60 plataformas sociales**  
Herramienta OSINT ligera, sin backend, con verificación manual de enlaces y tres temas visuales (Matrix, Claro, Ámbar).

> ⚠️ **Importante**: Introduce el nombre de usuario **sin el símbolo `@`**.  
> Ejemplo: `pepito` (no `@pepito`).

## ✨ Características

- 📋 **Más de 60 plataformas** (Twitter, Instagram, GitHub, TikTok, Steam, etc.)
- 🔗 **Enlaces directos** a cada perfil, generados automáticamente.
- ✅ **Verificación manual** de existencia: botón "Verificar" que comprueba si la URL responde (petición HEAD con timeout de 5 segundos).
- 🎨 **Tres temas**: Matrix (negro/verde), Claro (blanco/verde) y Ámbar (naranja retro).
- 📄 **Paginación** (25 resultados por página) para no saturar la pantalla.
- 💾 **Persistencia** del tema elegido (guarda en `localStorage`).
- 🚀 **Cero dependencias**: todo en un único archivo HTML/CSS/JS.
- 🔒 **Sin envío de datos**: toda la verificación es local, no requiere servidor.

## 📋 Lista de plataformas (algunas)

Twitter, Instagram, Facebook, LinkedIn, GitHub, Reddit, YouTube, TikTok, Twitch, Pinterest, Snapchat, Telegram, Discord, Spotify, Medium, DeviantArt, Flickr, Dribbble, Behance, Vimeo, SoundCloud, Tumblr, GitLab, Bitbucket, Keybase, HackerNews, ProductHunt, Mastodon, Steam, Codecademy, Dev.to, Gravatar, Pastebin, Replit, Codepen, LeetCode, HackerRank, Kaggle, ResearchGate, Academia.edu, Slideshare, Bandcamp, Last.fm, Foursquare, Untappd, Strava, Imgur, Giphy, VK, Weibo, Wattpad… y más.

## 🎨 Cambiar de tema

Usa los botones de la cabecera:  
🌙 **Matrix** | ☀️ **Claro** | 🟠 **Ámbar**  
El tema se guarda automáticamente para la próxima visita.

## 📁 Estructura del proyecto

repositorio/
├── social-lite.html # Aplicación completa (único archivo)
└── README.md # Este archiv


## ⚠️ Limitaciones

- La verificación con `fetch(..., {mode: 'no-cors'})` solo indica si el servidor responde, **no** si el usuario realmente existe. Por ejemplo, Twitter puede devolver una página de inicio de sesión en lugar de 404. Úsalo como orientación.
- No se resuelven captchas ni se simula navegador real.
- Algunas plataformas pueden tener cambios en sus URLs; si un enlace no funciona, repórtalo para actualizar la lista.

_Hecho para investigadores OSINT, periodistas y curiosos. Sin complicaciones, sin servidores._
