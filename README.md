# invitaciones-entregas

Acá viven las invitaciones digitales de **ventas reales** de Late. Separado a propósito del repo `invitaciones-digitales` (el catálogo público de demostración) — nunca se mezclan.

## Por qué existe este repo separado

El catálogo (`invitaciones-digitales`) muestra templates con datos de ejemplo y fotos de stock para que un cliente potencial vea el estilo. Una vez que alguien compra, la invitación *real* — con sus datos, sus fotos, su fecha — no puede vivir ahí. Este repo es donde entregás cada venta, y GitHub Pages lo publica en:

```
https://norbertoloyola.github.io/invitaciones-entregas/<carpeta-de-la-venta>/
```

## Cómo entregar una venta nueva

1. Copiá el template elegido del catálogo (`invitaciones-digitales/templates/<categoría>/...`) a una carpeta nueva acá, con este formato de nombre:
   ```
   nombre-evento-fecha/
   ```
   Ejemplo: `casamiento-maria-juan-2026-11-14/`

2. Personalizá el `CONFIG` del `index.html` copiado con los datos reales del cliente (nombres, fecha, lugar, mensaje).

3. Reemplazá las fotos de stock en `img/` por las fotos reales que te mande el cliente (mismo nombre de archivo, `foto-1.jpg`, `foto-2.jpg`, etc. — así no hay que tocar el código, solo los archivos).

4. **Cargá `RSVP_LOG_URL`** con la URL real del Apps Script (la misma para todas las ventas — está en `rsvp-apps-script.md` del repo del catálogo). Sin esto, el RSVP no queda registrado en ninguna planilla.

5. Confirmá que `whatsappNumero` en el `CONFIG` sea el número que el cliente te haya pasado para recibir las confirmaciones — nunca el tuyo ni el del catálogo (viene con un placeholder `5491100000000` que hay que reemplazar siempre).

6. Subí la carpeta (`git add`, `git commit`, `git push`).

7. **Probá el link vos mismo antes de mandarlo**: countdown corriendo bien, mapa apuntando a la dirección correcta, botón de WhatsApp al número correcto, fotos cargando, RSVP registrando en la planilla.

8. Mandale el link al cliente para que lo revise antes de compartirlo con sus invitados.

## Más adelante

Cuando haya ingresos reales, evaluar dominio propio corto (`tuinvitacion.com.ar/nombre-evento`) en vez de la URL larga de GitHub Pages — ver Fase 4 del `PLAN-COMERCIAL.md` en el repo del catálogo.
