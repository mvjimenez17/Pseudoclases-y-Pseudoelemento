# ::after 
_En CSS, ::after crea un pseudo-elemento que es el último hijo del elemento seleccionado. Es comunmente usado para añadir contenido cosmético a un elemento con la propiedad content.Es en linea (inline) de forma predeterminada._

/* Añade una flecha después de los enlaces */
a::after {
  content: "→";
}

# ::before
 _En CSS, ::before crea un pseudoelemento que es el primer hijo del elemento seleccionado. Es usado normalmente para añadir contenido estético a un elemento, usando la propiedad content. Este elemento se muestra en línea con el texto de forma predeterminada._

/* Añade un corazón antes de los enlaces */
a::before {
  content: "♥";
}

# ::first-letter (:first-letter)
_El pseudo-elemento ::first-letter aplica estilos a la primera letra de la primera línea un elemento de bloque, sólo cuando no es precedido de otro contenido (como imágenes o tablas)._

/* Selecciona la primera letra de <p> */
p::first-letter {
  font-size: 130%;
}

# ::first-line (:first-line)
_El Pseudoelemento ::first-line aplica estilos a la primera línea de un elemento de bloque. Nótese que la longitud de la primera línea depende de muchos factores, incluyendo el ancho del elemento, el ancho del documento y el tamaño de fuente del texto._

/* Selecciona la primera línea de un parrafo < P > */
p::first-line {
  color: red;
}

# ::selection
No estándar: Esta característica no es parte de los estándares. No la uses en sitios Web en producción: no funcionará para todos los usuarios. Podrían haber también incompatibilidades considerables entre distintas implementaciones y el comportamiento podría cambiar en el futuro.

Resumen
El selector ::selection CSS pseudo-elemento aplica reglas a una porción de un documento que ha sido destacado (por ejemplo: selección con el mouse o algún otro puntero en un dispositivo) del usuario.

Sólo un pequeño subconjunto de propiedades CSS pueden ser usadas en una regla ::selection en el selector de: color, background, background-color y text-shadow. Nótese que, en particular, background-image es ignorado, como cualquier otra propiedad.

# ::backdrop

_Cada uno de los elementos en la pila de la capa superior posee un ::backdrop pseudo-element. Este pseudo-elemento es una caja que se muestra inmediatamente debajo del elemento (y sobre el elemento inmediatamente inferior de la pila, si es que hay), dentro de dicha capa superior._

Nota: El pseudo-elemento ::backdrop se puede usar para crear un fondo que oculte el documento subyacente detrás de la pila de la capa superior, p.ej., para el elemento que es mostrado a pantalla complete tal y como se describe en esta especificación.

No se hereda ni es heredado de ningún elemento. Tampoco se hacen restricciones sobre qué propiedades se aplican a este pseudo-elemento.


# ::placeholder
El pseudo-elemento CSS ::placeholder representa el texto provisional en un elemento input o un elemento textarea.

::placeholder {
  color: blue;
  font-size: 1.5em;
}

Solo el subconjuto de las propiedades CSS que aplican al pseudo-elemento ::first-line puede ser usado en una regla utilizando ::placeholder en su selector.
# ::marker
Experimental: Esta es una tecnología experimental
Comprueba la Tabla de compabilidad de navegadores cuidadosamente antes de usarla en producción.

El pseudo-elemento ::marker en CSS selecciona la caja de marcadores de un elemento de la lista, que normalmente contiene una viñeta o un número. Funciona en cualquier elemento o pseudo-elemento configurado para display: list-item, como el elemento <li> y <summary> (en-US).

::marker {
  color: blue;
  font-size: 1.2em;
}
Copy to Clipboard
Propiedades permitidas
Sólo ciertas propiedades CSS puedes utilizarse en una regla con ::marker como selector:

Todas las propiedades de fuentes
color
La propiedad text-combine-upright (en-US), unicode-bidi (en-US) y direction
La propiedad ____content:'';__

#  ::spelling-error 

representa un segmento de texto que el user agent (en-US) ha marcado como deletreado incorrectamente.

::spelling-error {
  color: red;
}
Propiedades permitidas
Solo se puede usar un pequeño subconjunto de propiedades de CSS en una regla con ::spelling-error en su selector:

color
background-color
cursor
caret-color
outline y sus longhands
text-decoration y sus propiedades asociadas
text-emphasis-color
text-shadow

#  ::grammar-error 

representa un segmento de texto que el agente de usuario ha marcado como gramaticalmente incorrecto.

Propiedades permitidas
Solo se puede usar un pequeño subconjunto de propiedades CSS en una regla con ::grammar-errorsu selector:

color
background-color
cursor
caret-color
outliney sus manos largas
text-decorationy sus propiedades asociadas
text-emphasis-color
text-shadow

::grammar-error {
  text-decoration: underline red;
  color: red;
}


