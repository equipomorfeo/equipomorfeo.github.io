# Estudio Morfeo 🌙

Donde los sueños toman forma. Web principal del estudio.

## 🚀 Publicar en GitHub Pages

1. Crea un repositorio llamado **`estudiomorfeo.github.io`** en GitHub
2. Clona el repo y copia estos archivos en la raíz
3. Haz push a la rama `main` (o `master`)

GitHub Pages publicará automáticamente en:
→ **https://estudiomorfeo.github.io**

### Con GitHub Actions (alternativa)

Si prefieres mantener el código en un repo normal y desplegar a Pages:

```yaml
# .github/workflows/deploy.yml
name: Deploy to GitHub Pages
on:
  push:
    branches: [main]
jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: .
```

## 📁 Estructura

```
estudiomorfeo/
├── index.html          # Página principal
├── agentes.html        # Equipo de agentes
├── proyectos.html      # Proyectos del estudio
├── contacto.html       # Formulario de contacto
├── css/
│   └── estilo.css      # Estilos globales
└── README.md
```

## 🛠️ Tecnologías

- HTML5 semántico
- CSS3 (variables, grid, flexbox, responsive)
- Sin dependencias externas

## 📬 Contacto

- Web: [estudiomorfeo.github.io](https://estudiomorfeo.github.io)
- Email: hola@estudiomorfeo.dev
