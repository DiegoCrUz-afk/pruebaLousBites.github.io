# 🍪 Lousbite — Galletas Artesanales

Sitio web estático para **Lousbite**, emprendimiento de galletas artesanales. Construido para GitHub Pages con panel de administración vía Decap CMS.

## 🌐 Sitio en vivo

```
https://TU_USUARIO.github.io/NOMBRE_DEL_REPO/
```

## 📁 Estructura del proyecto

```
├── index.html              # Página principal — timeline de posts
├── catalogo.html           # Catálogo de productos
├── calendario.html         # Calendario mensual de ventas
├── css/
│   └── style.css           # Estilos (tema rosa/café)
├── js/
│   └── public.js           # Lógica del frontend — carga datos desde JSONs
├── data/
│   ├── productos.json      # Productos del catálogo
│   ├── posts.json          # Posts del timeline
│   └── calendario.json     # Eventos del calendario
├── admin/
│   ├── index.html          # Panel de administración (Decap CMS)
│   └── config.yml          # Configuración de Decap CMS
└── images/
    ├── logo.png            # Logo de Lousbite
    ├── personaje.png       # Mascota/personaje
    └── uploads/            # Imágenes subidas desde el admin
```

## 🛠️ Administración de contenido

El sitio usa **Decap CMS** para administrar productos, posts y calendario sin necesidad de backend.

### Para acceder al admin:
1. Andá a `https://TU_USUARIO.github.io/NOMBRE_DEL_REPO/admin/`
2. Iniciá sesión con tu cuenta de GitHub
3. Administrá productos, posts y fechas del calendario desde el panel

Los cambios se guardan como commits automáticos al repositorio. GitHub Pages despliega los cambios en 1-2 minutos.

### Configuración del OAuth (primer uso):
1. Creá una **OAuth App** en [GitHub Developers](https://github.com/settings/developers)
   - Homepage URL: `https://TU_USUARIO.github.io/NOMBRE_DEL_REPO/`
   - Callback URL: `https://oauth.decapcms.com/auth`
2. Registrá el **Client ID** y **Client Secret** en [Decap CMS OAuth](https://decapcms.com/oauth)
3. Actualizá `admin/config.yml` con tu usuario y nombre de repo

## 🚀 Deploy

El sitio es 100% estático — subilo a GitHub Pages:

```bash
git init
git add .
git commit -m "feat: sitio Lousbite con Decap CMS"
git remote add origin https://github.com/TU_USUARIO/NOMBRE_DEL_REPO.git
git push -u origin main
```

En GitHub: **Settings → Pages → Source: Deploy from branch `main`, root folder**.

## 🧪 Probar localmente

```bash
npx serve .
# o
python -m http.server 3000
```

Luego abrí `http://localhost:3000` en el navegador.

> ⚠️ El panel admin (`/admin/`) solo funciona en GitHub Pages, no en localhost.

## 📞 Contacto

- Instagram: [@lousbite](https://www.instagram.com/lousbite/)
- Teléfono: 3095-9661 / 5771-4771

---

🍪 Hecho con amor
