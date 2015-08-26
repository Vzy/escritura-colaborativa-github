# Gitbook

## Intro Gitbook

Gitbook es una plataforma online que nos permite escribir textos con el lenguaje Markdown y la tecnología git, de manera relativamente sencilla para la usuaria no experta en git o github, sin tener que usar la línea de comandos ni tener que instalar nada en nuestro ordenador. Podemos simplemente escribir, compartir, acutalizar y colaborar en la escritura de textos desde el navegador. El panel de escritura vía web permite visualizar la estructura del texto a la izquierda, escribir en el centro y ver el resultado de la interpretación visual del lenguaje de marcas a la derecha. El portal gitbook permite escribir un texto colaborativamente de manera asíncrona, usando el sistema de control de versiones y colaboraciones de git directamente a través de la web, de manera completamente transparente. Además Gitbook permite la publicación del libro, su venta y distribución online, todo de manera gratuita. Gitbook es, además, software libre y puede instalarse en otros servidores que no sean gitbook.com, por lo que no nos hace dependientes de una empresa. Además gitbook permite conectarnos automáticamente a github, y mantener nuestros repositorios de texto y código en la comunidad de github. Permite por tanto usar la tecnología git sin tener que dominar su uso o saber usar github, al tiempo que permite a otras personas que contribuyan al texto desde diferentes plataformas, desde su ordenador o desde su red de colaboración favorita (siempre que usen Git).

## Cómo conectar github con gitbook y viceversa

Conectar cuentas de gitbook y github

En la página de settings de gitbook [https://www.gitbook.com/@xabier/settings] vamos hacia abajo y nos encontramos con las opciones de permisos para github, allí escogemos la última "with access to private repositories", nos llevará a github y allí veremos tenemos que comprobar si tenemos también permiso para los webhooks. Pondrá " Full control of repository hooks" y "Access private repositories"

Crear nuevo libro en gitbook

Al crear el libro nos saldrá la opción de o bien empezar a escribir o bien conectarlo con github. No lo conectes a github, simplemente dale a editar, ahora gitbook creará la estructura básica del libro. Una vez hecho esto volvemos atrás al menú principal del libro. Ahora ya puedes ir a Settings y en el menún de la columna de la derecha abajo encontrarás un enlace que pone Github, haz click ahí.

En otra ventana y entrando en github, tienes que crear un proyecto (con el mismo nombre ayuda) en github, al hacerlo elegir .gitignore de gitbook (al lado de la licencia)

Enlazamos el (hay png) y luego nos aparecerá una opción de Add deployment webhook, hacemos click allí y guardamos.

NO FUNCIONA BIEN NADA DE ESTO, el webhook parece que se crea automáticamente, pero no hay manera, no sé si hay problemas o qué pasa.

Luego vamos al 

https://git.gitbook.com/xabier/comunes-conocimiento-democracia.git

