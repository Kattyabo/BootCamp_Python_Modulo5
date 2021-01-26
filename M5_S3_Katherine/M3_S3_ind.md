1. Qué es XSS y por qué es peligroso.

    Los ataques XXS son un tipo de inyección en la cual un atacante logra ejecutar código en los navegadores de los usuarios que acceden a un sitio web legítimo.     

2. Explique en qué consisten y las diferencias entre un requerimiento GET y un requerimiento POST y cómo son atendidos por Django.

    La diferencia entre los métodos get y post radica en la forma de enviar los datos a la página cuando se pulsa el botón “Enviar”. Mientras que el método GET envía los datos usando la URL, el método POST los envía de forma que no podemos verlos (en un segundo plano u "ocultos" al usuario).

3. ¿Cómo se comunica Django con el servidor HTTP utilizado para desplegar en producción un proyecto web?
    Django es un framework para desarrollo web pero hay muy poca información relacionada sobre como hacer despliegue o deploy (en ingles). Voy a explicar cómo llevar a producción una aplicación hecha en Django y una base de datos PostgreSQL, en un servidor web.

4. ¿Cómo son enviados, utilizando el protocolo HTTP, los datos generados por un formulario? Indique en qué sección del mensaje HTTP van incluidos estos datos.

    Un Formulario HTML es un conjunto de uno o más campos/widgets en una página web, que pueden ser usados para recolectar información de los usuarios para el envío a un servidor. Los formularios son un mecanismo flexible para recolectar datos de entrada porque son widgets adecuados para ingresar diferentes tipos de datos, incluyendo campos de texto, checkboxes, radio buttons, selector de fechas, etc. Los formularios son también una forma relativamente segura de compartir datos con el servidor, ya que permiten enviar información en peticiones POST con protección de falsificación de solicitud entre sitios.

5. Explique la función que cumple la etiqueta <form> en un documento HTML. Sus atributos action y method, ¿son necesarios? de ser asi ¿cuándo son necesarios?
    
    El elemento HTML form (<form>) representa una sección de un documento que contiene controles interactivos que permiten a un usuario enviar información a un servidor web.
    El elemento form inserta un componente diseñado para contener controles con los que el usuario puede interactuar para enviar información de regreso al servidor. Este elemento es comúnmente usado para recolectar información de los visitantes del sitio, como preferencias, comentarios, opiniones y muchas cosas más. También es muy importante en el proceso de acceso que muchos sitios web proveen.
    De todos sus atributos, dos tienen mayor importancia y son habitualmente utilizados: action y method. El atributo action indica la ubicación del programa que procesará la información enviada por el navegador, cuando el formulario sea despachado. Este programa está escrito en cualquier lenguaje del lado servidor y se supone que esté preparado para recibir y procesar los datos del formulario.
    Por otra parte, el atirbuto method indica cómo debe el navegador adjuntar los datos del formulario a la petición. Es recomendable usar el método "POST" debido a que éste oculta la información enviada y permite la transmisión de datos binarios. Sin embargo, algunas situaciones específicas pueden requerir el uso del método GET.
    Es posible usar las pseudo-clasess de CSS :valid e :invalid  para darle estilos a un elemento form.

6. Qué diferencia hay entre la validación de formularios realizada por ej: navegador web, validaciones a través de javascript y validaciones realizadas por el Framework Django. ¿En qué casos se ocupan las unas o las otras?
    
    Javascript se preocupa de enviar datos al servidor, es importante asegurarse de que se completan todos los controles de formulario requeridos, y en el formato correcto. Esto se denomina validación de formulario en el lado del cliente y ayuda a garantizar que los datos que se envían coinciden con los requisitos establecidos en los diversos controles de formulario.
    La validación de los campos de un formulario es una tarea de programación necesaria, aunque muchas veces es un proceso molesto. Para ejecutar la validación por parte del cliente es habitual recurrir a scripts, la mayoría de las veces en lenguaje JavaScript o emplear alguna librería para verificar que las entradas son del tipo correcto y que estén completas con datos, antes de que el formulario sea enviado. En HTML5 los nuevos atributos de las entradas como required y pattern usados en combinación con selectores de CSS, facilitan la programación y mejora de la interfaz del usuario.
    ormularios HTML en Django, y en particular, la forma más fácil de escribir formularios para crear, actualizar y borrar instancias de modelo.

7. El envío de datos de formulario se realiza con la acción submit de un elemento del documento HTML y en otros casos esa funcionalidad es anulada y en su lugar es realizada por código JavaScript. Investigue y explique por qué podría utilizarse una u otra forma. En qué casos usted preferiría uno u otro método.
    
    En cuanto a la diferencia entre buttony input:
    * A buttonpuede tener un valor separado como datos, mientras que para un inputlos datos y el texto del botón son siempre los mismos:
<input type="button" value="Button Text"> <!-- Form data will be "Button Text" -->
<button type="button" value="Data">Button Text</button>
    * A buttonpuede tener contenido HTML (por ejemplo, imágenes), mientras que an inputsolo puede tener texto.
    *A buttonpuede ser más fácil de diferenciar de otros inputcontroles (como campos de texto) en CSS. Tenga en cuenta la compatibilidad del navegador con versiones anteriores.

Katherine Barrera Ordenes