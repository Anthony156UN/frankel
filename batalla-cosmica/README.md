# Batalla Cósmica — V0.5 (beta multijugador)

**Nuevo tablero sin cuadros:** espacio continuo con estrellas, planetas flotantes y mano de 4 cartas en abanico. Los bordes propios de las cartas y el brillo dorado al elegir meteorito siguen presentes.

Juego de cartas espacial original, en fase de pruebas. **Nombre provisional**.

## Probar con un amigo
1. Abre el sitio publicado con GitHub Pages.
2. Pulsa **Crear sala privada** y comparte el enlace por WhatsApp.
3. El amigo abre el enlace; ambos deben mantener la página abierta.
4. El anfitrión pulsa **Comenzar partida**; las manos se mantienen privadas y las jugadas se sincronizan.

También hay **práctica contra bot**. La mano tiene **4 cartas**; puedes jugar una o descartar de 1 a 4 y robar automáticamente. Mazo central boca abajo, descarte boca arriba y remezcla automática al agotarse el mazo.

La **estrella fugaz** permite elegir solo una acción: **atacar, proteger o transformarse en el planeta deseado**. No hay restricciones por colores.

## Dónde está la demo
El juego está en `batalla-cosmica/index.html`. Si GitHub Pages publica `main / (root)`, la ruta esperada es:
https://anthony156un.github.io/frankel/batalla-cosmica/

Si no se abre, habilitar en el repositorio **Settings → Pages → Deploy from a branch → main / (root)**.

## Limitaciones de la beta
La conexión utiliza PeerJS Cloud para señalización y WebRTC entre navegadores. El anfitrión valida las jugadas, pero **no es aún un servidor competitivo seguro**. La conexión puede fallar por políticas de red o NAT, el anfitrión debe permanecer conectado y la partida no se guarda en la nube. Esta beta no incluye anuncios, clasificación ni registro.
