# Boxed in space

## Índice

1. **Historial de versiones**
2. **Introducción**
    - Concepto del Juego
    - Características principales
    - Género
    - Público objetivo
    - Estilo visual
3. **Mecánicas**
    - Jugabilidad
    - Objetos
    - Escenario
    - Flujo de juego
4. **Interfaz**
    - Diagrama de flujo
    - Menú principal
    - Créditos
    - Pantalla de selección de nivel
    - Nivel
    - Fin del juego
5. **Narrativa**
    - Premisa
    - Personajes
6. **Arte**
    - Concept art
    - Arte 2D
    - Arte 3D
7. **Audio**
    - Pistas
    - Efectos de sonido
8. **Roles del equipo**
  
---
## Historial de versiones

V 0.1: Primera versión del documento. Se ha establecido la base de todos los elementos.  
V 0.2: Segunda versión del documento. Se ha añadido la lista de objetos con sus mecánicas y descripciones.  
**V 0.3**: Tercera versión del documento. Se ha añadido la lista de objetos del escenario con sus mecánicas y descripciones.

## Introducción

### Concepto del Juego

En **Boxed in Space** encarnas a un ser que ha sido abducido por alienígenas. 
Celebrando su prosperidad económica y social, han decidido montar una fiesta en uno de sus más elegantes ovnis. Este año han decidido reunir a los seres más exóticos de la galaxia para exponerlos y así darle un toque especial a su fiesta. 
Tú eres uno de esos seres y debes regresar sano y salvo a tu hogar, descendiendo por todas las plantas de la nave.

### Características principales
- *Input* sencillo que permite jugar tanto en dispositivos móviles como en PC de forma cómoda.
- Dificultad seleccionable, dependiendo de la dificultad la nave madre será más grande o más pequeña (teniendo más niveles o menos).
- Variedad en los niveles gracias a la diversidad de objetos y sus distintas funciones.
- Requiere una combinación de habilidad e ingenio.

### Género
Videojuego tipo roguelike con elementos de puzzle.

### Público objetivo
Boxed in Space está enfocado tanto a jugadores habituales de “roguelikes” y puzles como a jugadores más casuales a los que pretendemos acercarnos con un estilo visual colorido y controles sencillos.

PEGI 3.

### Estilo visual
- Colores llamativos y fiesteros, pero con tonos un poco extraños (*alien*), que contrastan con el blanco y gris suave de la nave y sirven para dirigir la atención del jugador.
- Estilo de dibujo cartoon, los modelos 3D son realmente billboards que parecen recortes de papel.
- Diseño futurista/espacial mezclado con detalles de fiesta mundana (confeti, matasuegras …)

## Mecánicas

### Jugabilidad
- Deplazamiento: arrastrar el dedo por la pantalla del móvil en una de las 4 direcciones básicas hará que el cubo rote y se desplace una casilla en esa dirección.
- Objetos: los objetos estarán repartidos por las distintas casillas del tablero. Al colocarte sobre una de ellas el objeto se pegará a la cara inferior del cubo. Los objetos serán utilizados cuando queden en la cara superior del cubo.
- Interacción con el escenario: podrás usar elementos del escenario para ayudarte a avanzar.
- Cámara: se podrá desplazar la cámara alrededor del cubo para poder ver todas sus caras.
![Gameplay1](https://github.com/FormidableGames/boxed-in-space/blob/master/concepts/gameplay1.png "Movimiento")
![Gameplay2](https://github.com/FormidableGames/boxed-in-space/blob/master/concepts/gameplay2.png "Objetos")

### Objetos
- **Bomba confeti**: esta bomba que usan los aliens como petardo terrícola permite romper paredes resquebrajadas y elimina enemigos.   **Radio**: 1 casilla en todas las direcciones y diagonales.  
- **Deshidratador aurora**: con el gas a presión tan caliente que suelta deshiela suelo congelado y elimina enemigos. Los aliens lo usan para hacer bonitos efectos de nubes de colores.    **Radio**: 2 casillas en todas las direcciones.  
- **Bola de luces**: con la electricidad que alberga puede encender motores y elimina enemigos. Se usa para crear luces de colores como si se estuviese en una discoteca terrícola. Parece que estos aliens no saben crear aparatos de fiesta que no causen alguna clase de destrucción.    **Radio**: 3 casillas en la dirección de movimiento.  
- **Autodestructor**: si usas este objeto te eliminará instantáneamente, el motivo de crear un artilugio con este uso todavía me es desconocido. Creo que estos aliens no son tan inteligentes como parecen con su maquinaria avanzada.      **No tiene radio.**
  
### Escenario
- **Bloques resquebrajados**: Estos bloques funcionan como una pared normal pero pueden ser destruidos por la Bomba Confeti.  
- **Suelo helado**: Esta clase de suelo está cubierto por una capa de hielo que te hará deslizarte hasta que te choques con una pared o llegues a suelo normal. Al deslizarte solo contará como un turno de tu movimiento. Si una de estas casillas entra en el radio del Deshidratador Aurora volverá a ser suelo normal.  
- **Láseres**: Estos mortales artilugios sueltan haces de energía en linea recta que no se detendrán hasta que no se choquen con algo. Puede afectar tanto al jugador como a los enemigos. Su patrón de disparo es: disparo-carga-carga (empieza otra vez).
- **Puentes**: Caminos que se formarán solo si los activas de alguna manera.  
- **Baterías cortadas**: Fuentes de electricidad que han dejado de funcionar, si se les da una pequeña descarga eléctrica activarán un motor. Este motor podrá encender tanto puentes como láseres desactivados.  
- **Botones**: Al pulsarlos ocurrirá algo. Hay diferentes botones, dependiendo del icono que tengan harán una cosa u otra.  
    + Tipos:
       + Icono llave-puerta: abre la casilla de salida.
       + Icono copo de nieve: congela cierta parte del nivel. Las casillas que se puedan congelar tendrán marcas.  
       + Icono láser rotando: permite girar en 90 grados los láseres del nivel.
       + Icono camino: si hay un puente en el nivel (activo) al pulsar el botón este camino cambiará por otro distinto.
  
### Flujo de juego
Desde el menú podrás acceder al selector de dificultad. En el selector de dificultad podrás elegir entre tres dificultades: fácil, normal y difícil, además de un extra llamado *Custom* en el que podrás seleccionar tú mismo el número de salas y de vidas que tendrás durante el juego. Una vez en juego tendrás que ir avanzando con ayuda de los objetos que vayas encontrando por los distintos niveles buscando la salida, mientras evitas que los aliens te eliminen. Al acabar la partida aparecerán tus estadísticas y podrás volver al menú o reintentar el mismo nivel.

## Interfaz

### Diagrama de flujo
![Diagrama](https://github.com/FormidableGames/boxed-in-space/blob/master/concepts/Diagrama-flujo-aliens.png "Diagrama de flujo")

### Menú principal
![Menú](https://github.com/FormidableGames/boxed-in-space/blob/master/concepts/menu-principal.png "Menu principal")
1. Botones Jugar y Créditos. Jugar redirige a la pantalla del selector de nivel. 

### Créditos
![Créditos](https://github.com/FormidableGames/boxed-in-space/blob/master/concepts/creditos.png "Créditos")
1. Botón Volver (al menú principal).
2. Cubo de créditos: cada integrante del grupo aparece en una cara de un cubo que se puede rotar.

### Pantalla de selección de nivel
![Niveles](https://github.com/FormidableGames/boxed-in-space/blob/master/concepts/selector.png "Selección de nivel")
1. Botón Volver (al menú principal).
2. Barra de selección de nivel de dificultad. Cada nivel tiene unos parámetros determinados (número de salas y vidas) que determinará su dificultad. También se puede salir de estos estándares y personalizar el juego. 
3. Indicadores de los parámetros mencionados, con botones para modificarlos.
4. Botón Jugar.

### Nivel
![Nivel](https://github.com/FormidableGames/boxed-in-space/blob/master/concepts/nivel.png "Nivel")
1. Botones Reintentar y Pausa. El botón Pausa dará la posibilidad de volver al menú principal.
2. Zona de juego.
3. Botón Cámara. Con el modo cámara activado se podrá controlar la misma (dispositivos móviles).

### Fin del juego
![Final](https://github.com/FormidableGames/boxed-in-space/blob/master/concepts/fin-del-juego.png "Final")
1. Estadísticas del juego.
2. Botones Menú principal y Reintentar nivel.

## Narrativa

### Premisa
Un grupo de alienígenas va a montar un fiestón en su nave y para ello están recolectando a las especies más exóticas del universo. Eres una de esas especies, te han metido en una caja y no sabes qué quieren hacer contigo.

### Personajes
- **Cubo protagonista**: estás atrapado en una caja, lo único que sabemos de ti es que eres una de las especies más exóticas del universo.
- **Enemigos**: son los alienígenas que están preparando la fiesta, mejor que no te descubran.

## Arte

### Concept art
Nuestro protagonista:  
![Concept1](https://github.com/FormidableGames/boxed-in-space/blob/master/concepts/caja.png "Protagonista")    
![Concept2](https://github.com/FormidableGames/boxed-in-space/blob/master/concepts/caja2.png "Protagonista colorines")   
  
Un enemigo:  
![Concept3](https://github.com/FormidableGames/boxed-in-space/blob/master/concepts/alien.png "Enemigo")    

### Arte 2D
Siguiendo la estética visual establecida:
- Textura caja
- Iconos objetos
- Imagenes de aliens
- Objetos interactuables
- Iconos de la interfaz
- Fondos de la interfaz
- Botones del nivel
- Menús emergentes

### Arte 3D
- La caja
- Escenarios
- *Billboards*

## Audio 

### Pistas
- Menú principal.
- Música de la fiesta.
- Música victoria.
- Música derrota.

### Efectos de sonido
- Objetos.
- Enemigos.
- Movimiento.
- Navegación por menús.

## Roles del equipo
- **Sandra Valverde** - Programación.
- **Fco. Javier Vadillo** - Programación.
- **Sara López** - Diseño.
- **Nicolás Morales** - Arte 2D.
- **Guillermo Pitarque** - Arte 3D y sonido.
