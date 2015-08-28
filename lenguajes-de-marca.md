# Editores de texto y lenguajes de marcas

## Introducción

Desgraciadamente estamos demasiado aconstumbradas a los editores de texto tipo Word, o incluso Open/Libre Office, en los que no vemos el código que va por debajo de lo que escribimos. Vemos el resultado de una interpretación del texto que hay por debajo. Por decirlo de una manera sencilla tu ordenador sólo entiende el texto plano (sin negritas, ni tamaños de letra), pero cuando vemos un texto en un editor de texto normal vemos las letras con diferentes tamaños, colores, etc. El texto que hay por debajo es diferente. Por ejemplo la palabra "Hola", si aparece en negrita en nuetro editor de textos, probablemente esté codificada en texto plano en algo parecido a "<strong>Hola</strong>". Word convierte este código, originalmente en texto plano (sin formato), a negrita. Decía que desgraciadamente estamos demasiado acostumbradas a esto porque oscurece la estructura profunda del texto, el funcionamiento del programa, y dificulta también una colaboración "limpia" y ordenada en la producción de texto.

La alternativa a un editor de texto de este tipo es escribir directamente en un lenguaje de marcas. Los lenguajes de marcas son lenguajes, como los de programación, en los que directamente (sobre el mismo texto) especificamos una serie de propiedades del párrafo o de las palabras o letras: si están en negrita, si pertenencen al título, si son una nota al pié, si son el primer elemento de una lista numerada o si son una cita de un autor (por poner algunos ejemplos). Dicho de otro modo, un lenguaje de marcas permite que escribamos en un editor de texto plano (que no permite negritas o cursiva, etc.), como el Gedit o el Notepad, pero que podamos inmediatamente generar un documento (tipo pdf) en el que sí aparecen las negritas, o el texto justificado o los título a tamaño 16. 

HTML es un lenguaje de marcas, también LaTeX, o el lenguaje de marcas que se utiliza para la wikipedia. En general, los lenguajes de marcas han evolucionado hacia diferenciar las etiquetas que podemos llamar "identificativas" o de especificación, de las propiedades "estéticas" de esos elementos. Por ejemplo podemos usar la etiqueta "\<h1\>" para declarar que una cadena de texto es el título de una sección, así por ejemplo escribimos \<h1\>Qué es un lenguaje de marcas \</h1\> y al visualizar el documento la frase "Qué es un lenguaje de marcas" aparecerá como un tamaño determinado, centrado y en negrita, en forma de título. Lo más común es que las propiedades estéticas de las etiquetas estén definidas en otro documento que hace de plantilla de estilo, de tal modo que en el cuerpo de texto sólo definimos que "Qué es un lenguaje de marcas" es un título y en la plantilla definimos que los títulos de nivel 1 (\</h1\>) tienen un tamaño, color, márgenes, etc. determinados.

Lo bueno de estos lenguajes de marcas, es que sólo tenemos que concentrarnos en escribir el texto y en su estructura lógica o funcional, la estética vendrá después y podemos usar plantillas o diseños desarrolladas por otras personas o modificar el color de los títulos en la plantilla y que todo nuestro documento cambie automáticamente (esto se puede hacer con LibreOffice u otros editores al uso, pero poca gente comprender el funcionamiento de las plantillas y los estilos y la tendencia a cambiar directamente las propiedades de estilo de un párrafo o palabra nos impide ser sistemáticos, y de paso, dejamos el código subyacente al texto que vemos lleno de marcas innecesarias y engorrosas a la hora de trabajar colaborativamente con el texto). El control de versiones al usar un lenguaje de marcas es además mucho más eficaz y directo.

## Markdown y Pandoc

Uno de los lenguajes de marcas más populares y sencillos se llama Markdown. Es un lenguaje diseñado para ser fácil de usar, intuitivo, flexible, directo y rápido. Puedes consultar la sintaxis de Markdown en [DaringFireball](http://daringfireball.net/projects/markdown/syntax) o probar directamente en [Dillinger](http://dillinger.io), esta última web está dividida en dos columnas, en la de la izquierda puedes ver y editar directamente el texto plano en lenguaje Markdown y a la derecha verás cómo queda, la página de inicio ya cuenta con un texto que te permite aprender por imitación.

Con un editor de texto plano (como Gedit) puedes ya comenzar a usar markdown. Los documentos en Markdown llevan el sufijo ".md" de tal manera que el documento puede llamarse "introduccion.md". Puedes usar el editor de textos en Markdown [ReText](http://sourceforge.net/projects/retext/) para trabajar en local, puede hacer que se divida en dos de tal manera que escribes en el panel de la izquierda y a la derecha ves cómo va quedando el texto formateado.

    $ sudo apt-get install retext

Si tienes documentos ya escritos en Libre/Open Office o en otros formatos no te preocupes porque se pueden pasar a Markdown muy fácilmente. El programa que permite convertir texto en varios formatos a Markdown, y de Markdown a otros formatos (pdf, epub, odt, html, txt, etc.) se llama Pandoc. Pandoc es un programa de línea de comandos que nos permite interpretar Markdown (y otros lenguajes de marcas) y convertirlos a casi cualquier otro tipo de documento. Podemos instalarlo directamente:

    $ sudo apt-get install pandoc

Existen [infinidad de utilidades para usar pandoc](https://github.com/jgm/pandoc/wiki/Pandoc-Extras) que pueden facilitarte mucho la vida. Lo más normal es escribir un script (una pequeña secuencia de órdenes) para que de manera automática, tu texto en formato Markdown. 

## Usando Markdown y gestionando bibliografías



Pandoc
https://whk.name/cookbook/zoteroPandoc/


