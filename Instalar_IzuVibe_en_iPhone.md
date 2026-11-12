# Instalar IzuVibe en tu iPhone desde Windows

IzuVibe usa código de Trop v0.0.4 y conserva su licencia GPLv3. Necesita iOS 26.2 o posterior. La compilación crea un IPA sin firma: la firma personal se añade al instalarlo con tu cuenta Apple.

## Primera instalación y prueba

1. Instala iTunes. [La guía oficial de SideStore para Windows](https://docs.sidestore.io/docs/installation/prerequisites) enlaza las versiones de Apple y Microsoft Store; recomienda la de Apple.
2. Descarga **iloader estable** desde [su web oficial](https://iloader.app/). En Windows ofrece instalador MSI o EXE y permite importar un IPA propio.
3. Conecta el iPhone por USB, desbloquéalo y acepta **Confiar en este ordenador** en el teléfono.
4. Abre iloader, elige tu iPhone e inicia sesión con tu cuenta Apple. Introduce la contraseña y el código de verificación tú mismo dentro del programa.
5. Usa la opción de importar un IPA y selecciona `IzuVibe.ipa`. El programa lo firma para tu dispositivo y lo instala.
6. En el iPhone, sigue el aviso de confianza en **Ajustes → General → VPN y gestión de dispositivos**. Si pide **Modo de desarrollador**, está en **Ajustes → Privacidad y seguridad** y requiere reiniciar.
7. Abre **IzuVibe** desde su icono y prueba búsqueda y reproducción. Las funciones heredadas de Trop y el acceso al servicio musical necesitan verificarse en el dispositivo.

Con una cuenta Apple gratuita, la firma caduca a los siete días. Renueva antes de ese plazo. [FAQ oficial de SideStore](https://docs.sidestore.io/docs/faq).

## Mantenerla desde el iPhone con SideStore

Si quieres renovar desde el teléfono, la [guía oficial actual](https://docs.sidestore.io/docs/installation/install) usa iloader para instalar **SideStore (Stable)** inicialmente desde el PC. Después configura **LocalDevVPN** en el iPhone, inicia sesión en SideStore y renueva primero SideStore en **My Apps**. Importa luego el IPA de IzuVibe desde Archivos.

Para instalar, actualizar o renovar con SideStore hacen falta Wi-Fi y LocalDevVPN activo. La cuenta gratuita permite tres apps simultáneas, incluida SideStore. La renovación sigue siendo cada siete días; SideStore facilita hacerla desde el teléfono. Consulta los [requisitos](https://docs.sidestore.io/docs/installation/prerequisites) y la [FAQ](https://docs.sidestore.io/docs/faq) si aparece un error de emparejamiento.

## Comprobar la app instalada

- Buscar una canción por título y artista, abrir un resultado y reproducirlo completo.
- Probar pausa, siguiente, anterior, búsqueda dentro de la canción y segundo plano.
- Crear una playlist, añadir favoritos, cerrar y volver a abrir la app.
- Probar descargas con contenido cuyo proveedor y titular lo permitan, y comprobarlo sin conexión.
- Si falla, anotar el texto del error y la acción que lo provocó para corregirlo.

No se ha realizado una prueba física en tu iPhone. Compilar correctamente y reproducir música en el dispositivo son verificaciones distintas.
