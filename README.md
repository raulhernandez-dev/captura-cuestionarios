# Captura de cuestionarios en papel

Sitio estático para pasar a digital los cuestionarios en papel del estudio (Stunkard, Rosenberg, Birleson y KIDSCREEN-10). Gemini lee las fotos, tú revisas y exportas las filas en el mismo orden de columnas que Google Forms.

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (puede ser privado si tu plan lo permite; si es público, el código es visible, pero **no contiene datos ni la API key**).
2. Sube `index.html` a la raíz del repositorio.
3. En el repositorio: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, rama `main`, carpeta `/ (root)` → **Save**.
4. En 1–2 minutos el sitio queda en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`.

## Uso

1. Pega tu API key de Gemini (https://aistudio.google.com/apikey) y presiona **Cargar modelos**. Elige un modelo *Flash* (rápido y barato).
2. Sube las fotos de **un participante** (todas sus páginas) y presiona **Leer con IA**.
3. Revisa los campos en **amarillo** comparando con la foto (clic en la foto para hacer zoom) y presiona **Guardar participante**.
4. Repite con el siguiente participante.
5. Al terminar, presiona **Copiar filas para pegar en Excel** y pega en la primera celda vacía de la columna A de la hoja «Respuestas de formulario 1». Las fórmulas de calificación se aplican solas.

## Notas

- Los datos se guardan solo en el navegador donde capturas. Descarga un **Respaldo (JSON)** de vez en cuando; se puede restaurar en otro equipo.
- La IA devuelve vacío cuando una respuesta no es clara o tiene dos marcas: no adivina. Revisa siempre lo amarillo.
- Las fotos se envían a Google Gemini. Confirma con la persona responsable del estudio que está autorizado y no fotografíes nombres completos ni rostros.
- Si la API key es gratuita, Google puede usar los datos enviados para mejorar sus modelos; para datos sensibles conviene una key con facturación activa (nivel de pago).
