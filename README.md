# Wooddany Retratos · Catálogo de Obra

App web para gestionar el catálogo de obras de Wooddany Retratos.

## Contraseña de acceso
`wooddany2024`

Para cambiarla: abre `index.html`, busca la línea:
```
const PASSWORD = 'wooddany2024';
```
Y cambia el valor entre comillas por la contraseña que quieras.

---

## Cómo desplegar en Vercel (gratis)

### Paso 1 — Sube los archivos a GitHub
1. Ve a [github.com](https://github.com) y crea una cuenta gratuita si no tienes.
2. Crea un repositorio nuevo (botón verde "New").
3. Llámalo `wooddany-catalog`.
4. Sube los dos archivos: `index.html` y `vercel.json`.

### Paso 2 — Conecta con Vercel
1. Ve a [vercel.com](https://vercel.com) y entra con tu cuenta de GitHub.
2. Haz clic en "Add New Project".
3. Selecciona el repositorio `wooddany-catalog`.
4. Haz clic en "Deploy". En 1 minuto tendrás la URL lista.

### Paso 3 — Conectar tu subdominio de IONOS
En Vercel, ve a tu proyecto → Settings → Domains → añade `catalogo.wooddany.com`.

En IONOS, añade este registro DNS:
- Tipo: CNAME
- Nombre: `catalogo`
- Destino: `cname.vercel-dns.com`
- TTL: 3600

---

## Funcionalidades

- **Login con contraseña** — acceso privado
- **Panel de obras** — filtrado por año (2018–2026)
- **Nueva obra** — fotos desde el móvil o PC
- **Datos públicos** — número, año, tamaño, materiales (visibles en el dossier)
- **Datos privados** — cliente, fecha, precio, descripción (solo con QR)
- **Certificado de autenticidad** — generado automáticamente
- **QR descargable** — uno por obra, listo para imprimir
- **Dossier público** — filtrable por año, sin datos privados
- **Obras incompletas** — puedes guardar obras antiguas con los datos que tengas

## Almacenamiento

Los datos se guardan en el navegador (localStorage). Funcionan perfectamente para uso personal.

Si en el futuro quieres acceder desde varios dispositivos o compartir el catálogo con alguien más, el siguiente paso sería añadir una base de datos en la nube.
