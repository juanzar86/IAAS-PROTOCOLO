# Protocolo IAAS - Intervención Educativa Neonatal

Sitio estático (HTML/CSS/JS puro, sin build) con:
- Pre-test y post-test de conocimientos
- 5 módulos clínicos (video + PDF/presentación)
- 5 apartados de actualización (PDF)
- Comparación de resultados y descarga en CSV

## Estructura
```
index.html          <- página principal (todo el CSS/JS está embebido aquí)
images/             <- imagen de portada
modulo 1.../5/      <- imagen, video y PDF (o presentación) de cada módulo clínico
normativo.pdf
vigilancia.pdf
prevencion.pdf
fijaciones.pdf
alimentacion.pdf    <- material de los apartados de actualización
```

## Desplegar en Vercel
1. Sube esta carpeta a un repositorio de GitHub.
2. En Vercel: "Add New Project" → importa el repositorio.
3. Framework Preset: **Other** (sitio estático, no requiere build command).
4. Deploy.

## Nota sobre los videos
Los archivos .mp4 de los módulos son pesados (13-29 MB cada uno). GitHub los
acepta (ninguno supera 50 MB), pero si en el futuro crecen o agregas más,
considera subirlos a un servicio externo (YouTube no listado, Vercel Blob,
Cloudinary, etc.) y enlazarlos en vez de subirlos al repo.
