# IzuVibe para iOS â€” adaptaciÃ³n de Trop

Estado: cÃ³digo adaptado y preparaciÃ³n de compilaciÃ³n. **TodavÃ­a no compilado ni instalado en el iPhone.** Este ZIP no es un IPA instalable.

## Base y funciones reutilizadas

Base: SwiftyMedia/Trop v0.0.4, commit e44d95911d14e47ca77fb2ad7f7cafce8f90eca5.
https://github.com/SwiftyMedia/Trop/releases/tag/v0.0.4

Se conserva la bÃºsqueda y resoluciÃ³n nativa de YouTube Music mediante SwiftyTube/InnerTube; reproductor MPV, biblioteca, playlists, historial, letras, descargas, ecualizador y controles en segundo plano del proyecto original. No es una integraciÃ³n iTunes ni un iframe de la web. Esas funciones heredadas no se han verificado en tu dispositivo; dependen de servicios externos y pueden cambiar.
La documentaciÃ³n original pide cuenta YouTube Music mediante su web de inicio de sesiÃ³n dentro de la app; no afirma exigir Premium. No entregues contraseÃ±as en el chat. Los secretos de Last.fm que venÃ­an en el cÃ³digo se retiraron: esa integraciÃ³n opcional queda sin configurar. Discord conserva identificadores del proveedor original y no forma parte de las funciones configuradas de esta adaptaciÃ³n.

## Cambios de IzuVibe

- Nombre visible IzuVibe y bundle ID app.izuvibe.ios.
- Celeste #65d9ff, tema oscuro y fondo de reproductor negro por defecto.
- Icono de barras musicales; los iconos alternativos mantienen el sÃ­mbolo propio.
- Pantalla Acerca de con crÃ©ditos y licencia originales.
- Esquema compartido Xcode para compilaciÃ³n reproducible.
- Workflow manual que genera IzuVibe.ipa sin firmar. Se archivaron los workflows de publicaciÃ³n automÃ¡tica originales.
- El proyecto, mÃ³dulo y target internos siguen llamÃ¡ndose Trop para conservar sus rutas de compilaciÃ³n.

## Requisitos reales

El README original dice iOS26+, pero el proyecto de esta versiÃ³n exige **iOS26.2 o posterior**. Se conserva el requisito real del proyecto; no se redujo sin pruebas.
La compilaciÃ³n necesita macOS/Xcode. Desde Windows se puede ejecutar en un runner de GitHub. No hace falta comprar un Mac.

## Compilar desde Windows usando GitHub

1. Publica este cÃ³digo en un repositorio propio, conservando LICENSE.txt y los crÃ©ditos. Este paso NO se ha realizado por el asistente.
2. Para evitar costos, el workflow de este paquete solo corre en repositorios pÃºblicos con runner estÃ¡ndar. En un repositorio privado se omitirÃ¡ el job. Revisa siempre las condiciones vigentes de GitHub: https://docs.github.com/en/actions/concepts/billing-and-usage .
3. Abre Actions â†’ IzuVibe - compilar iOS â†’ Run workflow.
4. La primera compilaciÃ³n recompila FFmpeg y puede tardar bastante. No se disparÃ³ ninguna compilaciÃ³n ni se consumieron minutos durante la preparaciÃ³n local.
5. Al terminar, descarga el artefacto IzuVibe-iOS-sin-firmar y extrae IzuVibe.ipa.
6. Ese IPA requiere firma/instalaciÃ³n con AltStore Classic, SideStore u otro mÃ©todo compatible. No se instala desde Safari con un toque. Una cuenta gratuita de Apple requiere renovaciones periÃ³dicas; AltStore documenta siete dÃ­as.
   https://faq.altstore.io/altstore-classic/how-to-install-altstore-windows
   https://faq.altstore.io/altstore-classic/your-altstore

## Prueba previa del proyecto original

Para comprobar la reproducciÃ³n upstream antes de compilar cambios, el autor ofrece un IPA sin firmar en la release v0.0.4 enlazada arriba. Su feed puede estar desincronizado; usa la release estable directa. Ese IPA es Trop original, no la adaptaciÃ³n IzuVibe ni una compilaciÃ³n que haya hecho el asistente.

## Licencia y atribuciÃ³n

Trop, SwiftyMedia y colaboradores: GNU GPLv3, texto original en LICENSE.txt sin cambios.
Las modificaciones de esta adaptaciÃ³n se distribuyen bajo la misma licencia. Si redistribuyes binarios, debes cumplir sus condiciones y proporcionar el cÃ³digo fuente correspondiente. Esto no cambia los permisos ni tÃ©rminos del catÃ¡logo remoto.
Los avisos y copyright del cÃ³digo heredado permanecen intactos. README.md es el documento original. Los workflows/feed originales se conservan como referencia en upstream/.

## VerificaciÃ³n realizada

Se verificaron estructura del plist y esquema XML, JSON de los iconos, consistencia del target y referencias de assets, ausencia de la dependencia privada Discord Social SDK de main, conservaciÃ³n del archivo GPL y cambios de marca. No se ejecutÃ³ Xcode, no se generÃ³ IzuVibe.ipa y no se probÃ³ reproducciÃ³n, descarga o acceso a cuentas en el iPhone. La siguiente verificaciÃ³n necesaria es una compilaciÃ³n real de este cÃ³digo en macOS.
