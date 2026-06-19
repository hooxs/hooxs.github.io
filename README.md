# Mi Nido links

Sitio estatico usado por Mi Nido para enlaces publicos y App Links.

URL base:

- https://hooxs.github.io

Rutas de enlaces profundos:

- `/minido/verify-email?token=...`
- `/minido/reset-password?token=...`
- `/minido/family-invitation?token=...`

Documentos legales:

- `/legal/`
- `/legal/terminos-y-condiciones-mi-nido.pdf`
- `/legal/politica-tratamiento-datos-mi-nido.pdf`

## Android

`/.well-known/assetlinks.json` debe contener:

- Package: `com.hooxs.minido`
- SHA-256 del certificado real de firma de Android.

Pendiente antes de publicar: reemplazar `TODO_ANDROID_RELEASE_SHA256` por el SHA-256 de Google Play App Signing o del keystore release definitivo.

## iOS

`/.well-known/apple-app-site-association` queda sin asociaciones activas hasta tener:

- Apple Team ID.
- Bundle ID final de iOS.
- Associated Domains habilitado en Xcode/App Store Connect.
