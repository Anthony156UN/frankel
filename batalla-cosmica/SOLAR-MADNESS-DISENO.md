# SOLAR MADNESS — Diseño de los eventos cósmicos V0.6

**Estado: propuesta aprobable para implementación; las cinco cartas todavía NO son jugables en la V0.5.**
La beta actual sigue en `batalla-cosmica/index.html`. Diseño para dos jugadores, cuatro cartas en mano y cuatro planetas distintos sanos para ganar.

## Identidad y claridad

El Sol está fijo, los planetas reales elegidos para la propuesta son Tierra, Marte, Júpiter y Saturno; al jugar un planeta la carta se desintegra en partículas y el planeta se incorpora a su órbita. Los meteoritos parten del cinturón de asteroides visual del sistema; los asteroides decorativos no dan ataques gratuitos. Se indican los efectos con animaciones y una frase corta. El Sol y el cinturón no se roban ni intercambian.

## Nuevos eventos (10 cartas)

| Nombre | Copias | Poder 1 vs 1 | Animación |
|---|---:|---|---|
| Atracción Gravitacional | 3 | Mueve un planeta rival no protegido a tu sistema, con sus daños y accesorios. Requiere órbita de ese tipo libre. | Rayo tractor y nueva órbita |
| Intercambio Orbital | 3 | Entrega uno de tus planetas no protegidos a cambio de uno rival no protegido. Ambos deben quedar sin tipos repetidos. | Dos portales cruzados |
| Lluvia Errante | 2 | Transfiere hasta dos daños desde distintos planetas propios dañados hacia el mismo número de planetas enemigos sanos; cada objetivo se usa una vez. No se admite un objetivo protegido. | Meteoritos pequeños entre órbitas |
| Eclipse Total | 1 | El adversario descarta dos cartas aleatorias (o las que tenga) y las recupera por robo al comenzar su próximo turno, sin perder el turno. | Sol oculto y mano oscurecida |
| Inversión Cósmica | 1 | Intercambia los sistemas completos con accesorios y daños, incluso protegidos. Los soles y la habilidad solar pertenecen a sus dueños. La victoria derivada del intercambio se revisa al inicio del siguiente turno del beneficiario. | Dos sistemas cruzan un remolino |

**Protección:** para esta versión, un planeta con campo magnético activo no puede ser robado o intercambiado individualmente, y no puede recibir daños de Lluvia Errante. La luna sola no impide robo/intercambio. Inversión Cósmica es la excepción excepcional. Esto NO crea todavía una nueva carta de inmunidad.

**Partida rápida:** una carta por turno o descarte de hasta cuatro. Los poderes que requieren más de un objetivo mostrarán instrucciones paso a paso. No hay restricciones por colores. Las cartas especiales no requieren tener ya cuatro planetas; nunca permiten duplicar un tipo en el sistema.

## Mazo propuesto: 72 cartas

- Planetas: 28 (7 Tierra, 7 Marte, 7 Júpiter, 7 Saturno)
- Meteoritos: 11
- Campos magnéticos: 8
- Reparaciones: 7
- Lunas guardianas: 4
- Cometas: 2
- Estrellas fugaces: 2
- Eventos cósmicos: 10 (3 + 3 + 2 + 1 + 1)

Total: **72**. El motor actual de 72 cartas no cambia hasta que la implementación se pruebe. El Pulso Solar es habilidad separada, no carta del mazo. Las diez nuevas cartas sustituyen a 3 meteoritos, 2 escudos, 2 reparaciones, 1 luna y 2 cometas.

## Pruebas necesarias

1. Cada carta especial debe poder usarse desde celular sin instrucciones largas.
2. El servidor anfitrión valida y el rival no ve la mano privada ni las cartas restantes del mazo.
3. Nunca duplicar ni perder cartas al robar, intercambiar, descartar y reciclar el mazo.
4. Detectar victoria tras eventos en el momento convenido y bloquear jugadas inválidas.
5. Medir duración de partidas 1 vs 1 y comprensión de reglas con jugadores nuevos.

**Nota de originalidad comercial:** desarrollar redacción, ilustraciones y una combinación de habilidades distintivas, evitando replicar el conjunto completo de cartas y efectos de Virus!.
