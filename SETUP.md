# 🚀 Configuración de GitHub Pages

Esta guía te ayudará a configurar GitHub Pages para tu repositorio de Técnicas de Prompting para Periodistas.

## Requisitos Previos

- Cuenta de GitHub
- Repositorio creado con el contenido
- Git instalado localmente

## Paso 1: Preparar la Estructura

### 1.1 Crear carpeta docs
```bash
# En la raíz de tu repositorio
mkdir -p docs/assets/{css,js,images}
```

### 1.2 Copiar archivos principales
```bash
# Copiar index.html
cp index.html docs/

# Copiar configuración Jekyll
cp _config.yml docs/

# Copiar estilos y JavaScript
cp style.css docs/assets/css/
cp main.js docs/assets/js/
```

### 1.3 Estructura final
```
tu-repositorio/
├── docs/                    # Carpeta para GitHub Pages
│   ├── index.html          # Página principal
│   ├── _config.yml         # Config Jekyll
│   └── assets/
│       ├── css/
│       │   └── style.css
│       └── js/
│           └── main.js
├── es/                     # Contenido español
├── pt-br/                  # Contenido portugués
└── recursos/               # Recursos compartidos
```

## Paso 2: Configurar GitHub Pages

### 2.1 En GitHub.com

1. Ve a tu repositorio en GitHub
2. Click en **Settings** (⚙️)
3. Scroll hasta **Pages** en el menú lateral
4. En **Source**, selecciona:
   - **Deploy from a branch**
   - Branch: **main** (o master)
   - Folder: **/docs**
5. Click **Save**

### 2.2 Esperar el despliegue

- GitHub mostrará un mensaje: "Your site is ready to be published"
- El proceso toma 2-10 minutos
- URL final: `https://[tu-usuario].github.io/[nombre-repo]/`

## Paso 3: Personalización Opcional

### 3.1 Dominio personalizado

Si tienes un dominio propio:

1. Crea archivo `CNAME` en `/docs`:
```bash
echo "tudominio.com" > docs/CNAME
```

2. En tu proveedor DNS, configura:
   - Registro A apuntando a: `185.199.108.153`
   - Registro A apuntando a: `185.199.109.153`
   - Registro A apuntando a: `185.199.110.153`
   - Registro A apuntando a: `185.199.111.153`

### 3.2 Agregar Google Analytics

En `docs/index.html`, antes de `</head>`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

### 3.3 Favicon

Agrega tu favicon:
```bash
cp favicon.ico docs/
```

En `index.html`:
```html
<link rel="icon" type="image/x-icon" href="favicon.ico">
```

## Paso 4: Automatización con GitHub Actions

### 4.1 Crear workflow

Crea `.github/workflows/deploy.yml` con el contenido proporcionado.

### 4.2 Activar Actions

1. Ve a **Settings** → **Actions** → **General**
2. Selecciona **Allow all actions**
3. Save

## Paso 5: Mantenimiento

### 5.1 Actualizar contenido

```bash
# Editar archivos
git add .
git commit -m "Actualización de contenido"
git push origin main
```

### 5.2 Verificar estado

- Ve a **Actions** en tu repositorio
- Revisa el estado del workflow
- Check la página en vivo

## Solución de Problemas

### Error 404
- Verifica que la carpeta `/docs` existe
- Confirma la configuración en Settings → Pages
- Espera 10 minutos para propagación

### Estilos no cargan
- Revisa las rutas en `index.html`
- Usa rutas relativas: `./assets/css/style.css`

### Cambios no se reflejan
- Limpia caché del navegador (Ctrl+F5)
- Verifica que el commit se realizó
- Revisa Actions para errores

## Enlaces Útiles

- [Documentación GitHub Pages](https://docs.github.com/pages)
- [Jekyll Docs](https://jekyllrb.com/docs/)
- [Troubleshooting](https://docs.github.com/en/pages/getting-started-with-github-pages/troubleshooting-jekyll-build-errors-for-github-pages-sites)

## Soporte

Si encuentras problemas:
1. Revisa los [Issues](https://github.com/tu-usuario/tu-repo/issues) del repositorio
2. Crea un nuevo issue con detalles del error
3. Incluye capturas de pantalla si es posible

---

¡Felicidades! Tu sitio debería estar funcionando en GitHub Pages 🎉
