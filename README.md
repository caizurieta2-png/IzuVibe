# IzuVibe

App de música para iOS, con identidad celeste y negra, basada en **Trop v0.0.4** de SwiftyMedia y colaboradores. Conserva su licencia **GPLv3**.

## Código y compilación de IzuVibe

El código adaptado completo está en [IzuVibe_iOS_Fuente_Trop.zip](IzuVibe_iOS_Fuente_Trop.zip). La compilación de IzuVibe verifica el SHA-256 de ese paquete y compila su contenido. El árbol heredado de esta bifurcación se conserva como referencia de Trop; no se usa para generar IzuVibe.

- [Ejecutar o consultar la compilación de IzuVibe](https://github.com/caizurieta2-png/IzuVibe/actions/workflows/izuvibe-first-build.yml).
- [Guía del código nativo](IzuVibe_iOS_LEEME.md).
- Requisito del proyecto: **iOS 26.2 o posterior**.
- Nombre visible: **IzuVibe**; identificador: `app.izuvibe.ios`.
- Tema oscuro, acento `#65d9ff` e iconos propios.

El resultado es un **IPA sin firmar**. Su instalación requiere firma personal mediante una herramienta compatible; una cuenta Apple gratuita exige renovaciones periódicas. La reproducción y los servicios externos deben comprobarse en un iPhone real. No se promete un catálogo garantizado ni permisos de redistribución de la música.

## Créditos y licencia

IzuVibe adapta Trop v0.0.4, commit `e44d95911d14e47ca77fb2ad7f7cafce8f90eca5`. Los avisos originales y [LICENSE.txt](LICENSE.txt) se conservan. El código fuente correspondiente de esta adaptación se entrega en el ZIP enlazado. Trop pertenece a sus autores; IzuVibe no es un cliente oficial de YouTube, Spotify ni Apple.

<details>
<summary>Documentación original de Trop, como referencia</summary>

# Trop

A free and open source YouTube Music client for iOS.

<p>
	<img src=".github/assets/1.png" width="25%" alt="Homepage" />
	<img src=".github/assets/2.png" width="25%" alt="Player" />
	<img src=".github/assets/3.png" width="25%" alt="Queue" />
</p>

## Features

- No ads
- SponsorBlock: skips sponsor reads, intros, outros and non-music sections (silence, talking)
- Stream songs and videos from YouTube Music
- Synced lyrics (Musixmatch, Netease, Kugou, LRCLIB, Genius)
- Library sync (playlists, albums, artists, podcasts)
- Downloads
- Equalizer
- Custom app icons and themes
- Queue management and listening history

## Installation

Requires iOS 26 or later and a YouTube Music account (sign in through the in-app web view).

### Feather / AltStore / SideStore

Add the Trop source, then install the latest stable release (unsigned - your client re-signs it with your Apple ID):

```
https://raw.githubusercontent.com/SwiftyMedia/Trop/main/altstore.json
```


> **Note:** AltStore PAL is not supported.

Stable releases are available from the [releases page](../../releases). Nightly builds are available in the[Actions](../../actions) tab.

### Manual Installation

 To build an unsigned IPA locally, run `./build_ipa.sh`; the output is `build/Trop.ipa`.

## Notable mentions

- [InnerTubeX](https://github.com/MetrolistGroup/innertubex) - eXtended InnerTube API library for Kotlin
- [zemer-cipher](https://github.com/ZemerTeam/zemer-cipher) - YouTube cipher deobfuscation and PoToken generation
- [Metrolist](https://github.com/MetrolistGroup/Metrolist) - YouTube Music client for Android

## Community

Join the [Discord server](https://discord.gg/QrMwZAfU97) for support and discussion.

## License

This repo is licensed under [GPLv3](LICENSE.txt). Trop is not affiliated with, endorsed, or sponsored by Google or YouTube.


</details>

