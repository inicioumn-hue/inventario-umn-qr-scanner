# Escáner QR en vivo · Inventario UMN

Página estática de bajo costo para usar la cámara en vivo en teléfonos. El HTML Service de Google Apps Script bloquea el acceso directo a `getUserMedia`, por eso esta página se aloja aparte. El inventario, la hoja y las reglas de acceso siguen en Apps Script.

## Privacidad

- La página no recopila ni envía video o imágenes.
- El lector QR corre localmente en el navegador con jsQR (licencia Apache 2.0, incluida).
- Al leer un QR válido, el navegador abre el web app de Apps Script con el ID como parámetro. El inventario vuelve a aplicar sus permisos de Google.
- El código fuente de este escáner es público; no contiene la hoja ni claves del Backend.

## GitHub Pages

En el repositorio, configura **Settings → Pages → Deploy from a branch → main → /(root)**. Espera a que GitHub publique la página y comprueba que `https://inicioumn-hue.github.io/inventario-umn-qr-scanner/` abra el escáner por HTTPS.