# PRUEBA---RA2-HTML-CSS

 Ejercicio 1
Observa este HTML y CSS:

<header class="site-header">
  <h1>Mi Sitio Web</h1>

  <nav class="main-nav">                  HTML
      ...
  </nav>
</header>

.site-header {
  display: flex;
  justify-content: space-between;        CSS
  align-items: center;
}

h1 {
  text-align: center;
}

1A. Pregunta
¿Por qué NO se centra el texto del <h1> en este caso? Explícalo con tus palabras. (por qué visual y estructuralmente no aparece centrado entre el borde izquierdo y el menú)

1B. Ejercicio - Soluciona de dos formas diferentes

Debes indicar dos formas diferentes de conseguir que el h1 si quede centrado visualmente en la cabecera.

⚠️ IMPORTANTE:

Una solución usando Flexbox
Otra usando CSS Grid
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

1D. Ejercicio – Dar relieve y separación visual al header
Se pretende que la cabecera del sitio (.site-header) tenga un aspecto más definido y se diferencie claramente del resto de la página.

Debes conseguir, únicamente con CSS, que:

La cabecera tenga un color de fondo distinto al del resto de la página.
Haya una separación visual clara con el contenido que va debajo (por ejemplo, usando un borde inferior y una sombra).
El contenido del header tenga un espaciado interior adecuado para que no quede “pegado” a los bordes.
Escribe las reglas CSS que aplicarías a .site-header para lograr ese efecto.

