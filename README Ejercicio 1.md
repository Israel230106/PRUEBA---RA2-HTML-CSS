# PRUEBA---RA2-HTML-CSS

 Ejercicio 1
Observa este HTML y CSS:

<header class="site-header">
  <h1>Mi Sitio Web</h1>

  <nav class="main-nav"> 
      ...
  </nav>
</header>

.site-header {
  display: flex;
  justify-content: space-between;  
  align-items: center;
}

h1 {
  text-align: center;
}

1A. Pregunta
¿Por qué NO se centra el texto del <h1> en este caso? Explícalo con tus palabras. (por qué visual y estructuralmente no aparece centrado entre el borde izquierdo y el menú)

el <h1> está dentro de un contenedor flex (.site-header) que distribuye el espacio horizontal entre sus hijos, no dentro del <h1> mismo. Estohace que h1 este pegado a  la izquierda y nav esté pegado a la derecha. <h1> solo ocupa el espacio necesario para su contenido 

1B. Ejercicio - Soluciona de dos formas diferentes

Debes indicar dos formas diferentes de conseguir que el h1 si quede centrado visualmente en la cabecera.

⚠️ IMPORTANTE:

Una solución usando Flexbox

Usamos position: absolute y un flex (flex: 1) Así, aparte de centrar <h1>, mantenemos el menú con su tamaño normal.


CSS

.site-header {
  display: flex;
  align-items: center;
}

.site-header h1 {
  flex: 1;
  text-align: center;
}



Otra usando CSS Grid

Convertimos el header en una cuadriculade 3 columnas.

[auto]   [1fr]   [auto]


CSS

.site-header {
  display: grid;
  grid-template-columns: auto 1fr auto;
  align-items: center;
}

.site-header h1 {
  grid-column: 2;
  text-align: center;
}

En cada caso debes escribir:

Una breve explicación de la idea,
El CSS necesario para lograr el centrado.

1C. Ejercicio – Convertir la cabecera en dos filas

Sin modificar el HTML, debes conseguir mediante CSS que la cabecera se reorganice de la siguiente forma:

En la primera fila se muestra solo el <h1>, centrado horizontalmente.
En la segunda fila se muestra el menú de navegación (<nav class="main-nav">), también centrado horizontalmente.
Ambos elementos forman parte del mismo header, solo cambia la distribución.
Entre la fila del h1 y la fila del menú debe haber exactamente 30px de separación vertical (No puedes añadir etiquetas nuevas en el HTML. Solo se permite modificar el CSS)
Escribe el CSS necesario para conseguir esa estructura.

Usamos CSS Grid en 2 filas.

CSS:
.site-header {
  display: grid;
  grid-template-rows: auto auto;
  row-gap: 30px;
  justify-items: center;
}

.site-header h1 {
  grid-row: 1;
}

.site-header .main-nav {
  grid-row: 2;
}

1D. Ejercicio – Dar relieve y separación visual al header

Se pretende que la cabecera del sitio (.site-header) tenga un aspecto más definido y se diferencie claramente del resto de la página.

Debes conseguir, únicamente con CSS, que:

La cabecera tenga un color de fondo distinto al del resto de la página.
Haya una separación visual clara con el contenido que va debajo (por ejemplo, usando un borde inferior y una sombra).
El contenido del header tenga un espaciado interior adecuado para que no quede “pegado” a los bordes.
Escribe las reglas CSS que aplicarías a .site-header para lograr ese efecto.


CSS
.site-header {
  background-color: #f5f5f5;
  border-bottom: 2px solid #ddd;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  padding: 20px 0;
}
