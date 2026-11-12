# IzuVibe para iOS — primera compilación

**Compilación completada correctamente el 12 de noviembre de 2026 UTC.** El archivo `IzuVibe.ipa` está generado y sin firmar. Todavía no se ha instalado ni probado en tu iPhone.

## Resultado verificado

- [Ejecución de GitHub Actions](https://github.com/caizurieta2-png/IzuVibe/actions/runs/43149156842): finalizó con `success` y `BUILD SUCCEEDED`.
- Fuente ejecutada: commit `4d80f6ea3366a61d891a2bdb04552857b220295d`, que compila el ZIP adaptado verificado mediante SHA-256.
- Nombre visible: **IzuVibe**. Bundle ID: `app.izuvibe.ios`.
- Requisito real del binario: **iOS 26.2 o posterior**. Arquitectura: **arm64**, para iPhone físico.
- IPA: **47.292.257 bytes**. SHA-256: `2291ca86ece852c2835eeae13d1f89bf5240538733b0e5bec41a85e86eb2a578`.
- Pasaron CRC del ZIP, identidad del plist, formato Mach-O arm64, presencia de ejecutables de frameworks y ausencia de colisiones de rutas entre mayúsculas y minúsculas.

Estas comprobaciones verifican el archivo y su compilación. La reproducción, las descargas, el acceso a cuentas y el comportamiento en segundo plano requieren una prueba en el iPhone.

## Código publicado

Repositorio público: https://github.com/caizurieta2-png/IzuVibe

El código adaptado completo está en `IzuVibe_iOS_Fuente_Trop.zip`, en el repositorio y en esta carpeta. El árbol heredado de la bifurcación corresponde a Trop y se conserva como referencia; el workflow de IzuVibe compila el contenido del ZIP, no ese árbol heredado.

SHA-256 del ZIP de código: `d54443460b1a916b0d634b5bc089fbef26a09331ca5044f8b40050e6f9d8dd99`.

Base: [SwiftyMedia/Trop v0.0.4](https://github.com/SwiftyMedia/Trop/releases/tag/v0.0.4), commit `e44d95911d14e47ca77fb2ad7f7cafce8f90eca5`. Se conserva **GPLv3**, su archivo `LICENSE.txt`, los avisos originales y los créditos visibles en Acerca de. La documentación dentro del ZIP es la instantánea preparada antes de ejecutar esta compilación; este documento actualiza el resultado.

## Cambios propios y funciones heredadas

Nombre IzuVibe, identificador propio, celeste `#65d9ff`, tema oscuro, fondo de reproductor negro, iconos de barras musicales y créditos a Trop.

Se conserva la búsqueda y resolución nativa de YouTube Music de Trop, reproductor MPV, biblioteca, playlists, historial, letras, descargas, ecualizador y controles en segundo plano. Son funciones heredadas pendientes de verificación en el dispositivo y dependientes de servicios externos. La documentación original pide una cuenta YouTube Music dentro de la app; no afirma exigir Premium. La integración opcional de Last.fm queda sin credenciales configuradas.

## Repetir la compilación desde Windows

En el repositorio, abre **Actions → IzuVibe - Primera compilacion iOS → Run workflow**. El flujo usa un runner estándar público de macOS y genera el artefacto `IzuVibe-iOS-sin-firmar`, con el IPA y su checksum. FFmpeg quedó guardado en caché después del primer build. [Condiciones vigentes de GitHub Actions](https://docs.github.com/en/actions/concepts/billing-and-usage).

## Instalar

Sigue `Instalar_IzuVibe_en_iPhone.md`. El IPA necesita firma personal mediante una herramienta compatible. No requiere comprar un Mac; con una cuenta Apple gratuita la firma dura siete días y debe renovarse. La instalación y los inicios de sesión se completan en tus dispositivos.
