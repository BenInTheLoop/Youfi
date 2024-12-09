# 🎵 YouFi

Este proyecto permite transferir las canciones de una playlist de Spotify a una playlist en YouTube Music de forma automática.

## 🚀 Características

- Autenticación automática con Spotify y YouTube Music.
- Crea una playlist en YouTube Music si no existe.
- Busca y transfiere canciones desde Spotify a YouTube Music.
- Manejo de errores para evitar interrupciones.

---

## 🛠️ Requisitos

Antes de comenzar, asegúrate de tener los siguientes requisitos:

1. **Python 3.7 o superior**  
   Descárgalo desde [python.org](https://www.python.org/downloads/).

2. **Pip** (gestor de paquetes de Python)  
   Incluido con la mayoría de las instalaciones de Python. Si no lo tienes, instálalo siguiendo esta [guía oficial](https://pip.pypa.io/en/stable/installation/).

3. **Bibliotecas necesarias (SpotiPy & YTMusicApi) **  
   Instala las dependencias con el siguiente comando:

   ```bash
   pip install spotipy ytmusicapi

## ⚙️ Configuración del proyecto
1. Spotify API

    Ve a la consola de desarrolladores de Spotify y crea una nueva aplicación.

    Copia el Client ID y Client Secret.

    Reemplázalos en el código:
   ```bash
    SpotifyClientCredentials(
        client_id='TU_CLIENT_ID',
        client_secret='TU_CLIENT_SECRET'
    )

3. YouTube Music API

    Instala y configura las credenciales siguiendo los pasos:
      1. Abre YouTube Music en tu navegador.
      2. Inspecciona las solicitudes del navegador (F12 → Red → Filtrar por browse).
      3. Copia los headers (RAW) de una solicitud y pégalos en el terminal cuando el script lo solicite.
      4. El script generará automáticamente un archivo browser.json para futuras autenticaciones.
  
  ---
## 📖 Notas importantes
  Limitaciones de búsqueda: Es posible que algunas canciones no se encuentren debido a diferencias entre las plataformas.
    Tiempos de espera: El script utiliza un retraso de 5 segundos para evitar bloqueos por demasiadas solicitudes. Puedes ajustarlo según tus necesidades.

## ❤️ Contribuciones

Si deseas mejorar este proyecto, siéntete libre de abrir un issue o enviar un pull request. ¡Toda contribución es bienvenida!
