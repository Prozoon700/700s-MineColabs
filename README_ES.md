<p align="center"><img src="https://github.com/thecoder-001/MineColab/blob/master/Logo.png" alt="Logo" height="80"/></p>
<h1 align="center">700's MineColabs</h1>
 <p align="center">
   <img src="https://img.shields.io/badge/ESTADO-EN%20DESARROLLO-green">
   <img src="https://img.shields.io/github/stars/prozoon700?style=social">
</p>
<p align="center">
Esta es una versión modificada de MineColab (original por: <a href="https://github.com/thecoder-001/MineColab">thecoder-001</a>), optimizada, preparada para Forge y "con una interfaz gráfica".
Esta versión fue creada por Prozoon700 y originalmente hecha en español.
</p>
<h4 align="center">
:construction: Proyecto en desarrollo, si encuentras algún problema o tienes alguna sugerencia, por favor añádelo en el <a href="https://github.com/Prozoon700/700s-MineColabs/issues">área de issues</a>
</h4>
<p align="center"><a href="https://colab.research.google.com/github/Prozoon700/700s-MineColabs/blob/main/700s-MineColabs.ipynb" target="_parent"><img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" alt="Abrir en Google Colab"></a></p>
<br>

## :hear_no_evil:  Primero que todo, ¿qué es Google Colab?
Como dice la FAQ oficial, colaboratory, o "Colab" para abreviar, es un producto de Google Research. Colab permite a cualquier persona escribir y ejecutar código Python arbitrario a través del navegador, y es especialmente adecuado para el aprendizaje automático, el análisis de datos y la educación. Más técnicamente, Colab es un servicio de cuadernos Jupyter alojado que no requiere configuración para usar, y proporciona acceso gratuito a recursos computacionales, incluidos GPUs.
En resumen, es una máquina virtual proporcionada para aprender, ejecutar código Python, aprendizaje automático o para propósitos generales.

## :moneybag:  ¿Es realmente gratis de usar?
Sí, Colab es gratis de usar. Pero hay algunos puntos que, según yo, uno debería tener en cuenta:
1. Aunque Colab es un servicio gratuito, no debe explotarse indiscriminadamente o sin cuidado. Se debe valorar que es un recurso ofrecido sin costo y puede agotarse/restringirse si la demanda aumenta fuera de control.
2. Si no es obvio, no se deben ejecutar servicios críticos (como servidores grandes e importantes, bases de datos/programas Python) en él. Sus recursos no están garantizados ni son ilimitados, y los límites de uso a veces fluctúan. Además, el cuaderno tiene un tiempo máximo de ejecución de 12 horas, después de lo cual debe reiniciarse manualmente.
3. Si necesitas usarlo con frecuencia para tareas intensivas, considera comprar un servidor VPS. Un aumento significativo en la carga del servidor obligaría a Google a cerrar el servicio.

Al final, esta es solo mi opinión personal y puede ignorarse con seguridad. Simplemente pregúntale a tu corazón qué es lo correcto y qué es lo incorrecto. Además, por favor intenta usarlo como un recurso ocasional y no 24x7 para que otros también puedan aprovechar los recursos gratuitos.

# :hammer: Características
 - **Compatibilidad con Forge:** MineColab ahora es compatible con casi cualquier versión de Forge.
   - *¿Qué significa?* Ahora puedes incluir mods en tus servidores. Importante: Produce Lag y Ping de 1 a 4 segundos de retraso en el tiempo de respuesta.
   - Probado con versiones de Minecraft: 1.12.2, 1.18.2, 1.20.1, 1.20.2
   - Probado con versiones de Forge: 14.23.5.2859, 40.2.0, 47.2.0, 48.1.0

 - **Mejora de rendimiento:** Después de mucho tiempo de desarrollo y búsqueda, he optimizado el servidor con Flags de Java, mejorando considerablemente el rendimiento.
   - *¿Qué significa?* Ahora el servidor funciona mejor, normalmente no tiene lag ni retraso en la respuesta (Jugando con Paper).

 - **Creación de una interfaz gráfica:** He creado una "Interfaz de Usuario" para que la creación y en general todos los pasos sean más simples y visuales para los creadores.
   - *¿Qué significa?* Ahora en lugar de modificar código, simplemente agregarás valores a algunos campos que se ven visualmente.

 - **Personalización ampliada:** Ahora puedes personalizar cosas secundarias como los nombres de las carpetas y las regiones.
   - *¿Qué significa?* Ahora puedes tener todo "más organizado" y configurado a tu gusto.

# :page_with_curl: Instrucciones
1. Primero ejecuta la celda "Creación de los archivos necesarios" introduciendo los datos que vas a usar (Tipo de Servidor, Versión de Minecraft, Versión de Forge (en caso de usar Forge) y el Nombre del Directorio, donde se guardarán los archivos del servidor.), verificando primero que todo sea correcto.
   <br>
   - Tipo de Servidor -> Introduce el software que quieres que ejecute el servidor.
     - Vanilla (sin mods, pero con plugins) es "Paper".
     - Forge (sin plugins, pero con mods de Forge) es "Forge".
     - Fabric (sin plugins, pero con mods de Fabric) es "Fabric".
     - ¡Se agregarán más software tan pronto como sea posible!
   - Versión -> Aquí necesitarás poner la versión de Minecraft que va a usar tu servidor.
   <br>
   <br>
2. Luego ejecuta de nuevo la celda (Creación de los archivos necesarios) y esta vez debería tardar más, porque todos los archivos están siendo creados y montados.
   <br>
   <br>
3. Ahora necesitarás agregar un secreto al Cuaderno de Colab (Proyecto), para esto ve al menú del lado izquierdo y haz clic en el ícono de llave.
   - Agrega un nuevo secreto con los siguientes datos:
     - Nombre: server_directory
     - Valor: `Mostrado en la terminal`
   - Verifica que el cuaderno (proyecto) tenga acceso al secreto activando el interruptor.
5. Ahora que tus archivos han sido creados puedes verificarlos yendo al final (Visualizar los archivos de la carpeta) y ejecutando la celda o verificando el valor booleano del visualizador.
   <br>
   <br>
6. Después de esto, ve al principio hasta el tema "Iniciando el servidor" y llena los campos con los datos necesarios.
   - Versión de OpenJDK (Java) -> Introduce la versión de OpenJDK (Java) que necesitas para ejecutar tu servidor.
     - Si no sabes qué versión de OpenJDK necesitas usar, ve al tema "¿Qué versión de OpenJDK necesito?" e introduce tu versión de Minecraft siguiendo los pasos en la descripción del campo.
   - Servicio de agente -> Este campo es donde necesitas decidir qué agente estás usando. Cada agente tiene sus propios beneficios y desventajas.
     <br>
     | Nombre del Agente  | Facturación | Enlace | Pros | Contras |
     | ------------- | ------------- | ------------- | ------------- | ------------- |
     | `Ngrok`  | Parcialmente Gratis | [Web](https://ngrok.com)  | - Cambio de región gratuito. <br> - Mejor conectividad y tiempos.  | - Transferencia de datos limitada a 1 GB. <br> - Retraso en la renovación de la transferencia de datos de 1 mes. |
     | `PlayIt`  | Gratis | [Web](https://playit.gg)  | - Transferencia de datos ilimitada. <br> - Conexión sencilla del tablero. | - Región global, premium para cambiar. <br> - Peor conectividad y tiempos en algunos casos.  |
     | `Cloudflared` | Gratis y de pago | [GitHub](https://github.com/cloudflare/cloudflared) | - Transferencia de datos ilimitada. <br> - Múltiples subdominios. | - Difícil de instalar. <br> - Necesitas un dominio. |
     
      *El tema de facturación asegura que puedes jugar mayormente bien sin pagar nada.
   - Región -> Solo necesario cuando se usa el agente ngrok.
   - PlayitMessages (1,2,3) -> Solo necesario cuando se usa PlayIt y se quieren eliminar los mensajes personalizados que PlayIt envía a la consola.
   <br>
7. Cuando todos los campos necesarios estén llenos, ejecuta la celda (Iniciando el servidor) y si todos los pasos fueron seguidos correctamente, el servidor debería iniciar.
   <br>
   <br>
8. Para detener tu servidor, primero intenta ejecutar el comando stop en la terminal.
   - Si el servidor se reinicia (después de confirmar que los mundos y los datos están guardados), puedes forzar la detención del servidor deteniendo la ejecución de la celda.

# :question: Preguntas Frecuentes (FAQ)
- El servidor no se inicia.
  - Verifica si los archivos han sido creados.
    - Si solo se ha creado el archivo server.jar, vuelve a ejecutar la celda "Creación de los archivos del servidor".
    - Si no se ha creado ningún archivo, verifica que el software y las versiones estén correctamente escritos y existan en las páginas web de Paper, Forge, Fabric, etc.
    - Si todos los archivos han sido creados pero el servidor no se inicia, sigue leyendo.
  - Verifica que la configuración en la celda "Iniciando el servidor" sea correcta y no tenga errores de escritura.
    - Si algo está mal, detén el servidor si está en ejecución, cambia el valor, guarda los datos y vuelve a ejecutar el servidor.
    - Si todo está correcto, verifica que la versión de Java sea la correcta.
    - Si todas las configuraciones son correctas y la versión de Java es la adecuada, verifica la terminal en busca de errores y pégalos en la [Página de Issues](https://github.com/Prozoon700/700s-MineColabs/issues).
 - Verifica que Google Colab tenga permiso para acceder a Google Drive.
   - Si no es así, debería solicitarse, concede el permiso a Google Drive si quieres que el servidor funcione.
   - Si tiene permiso, verifica la terminal en busca de errores y pégalos en la [Página de Issues](https://github.com/Prozoon700/700s-MineColabs/issues).
- Los archivos del servidor no se crean
  - Verifica los valores de entrada de configuración
    - Si hay algo mal, detén la celda haciendo clic en el botón cuadrado en el lado izquierdo de la celda, modifica lo que necesites y vuelve a ejecutar la celda.
    - Si todo está bien, sigue leyendo.
  - Verifica que el directorio del servidor esté en un secreto con el nombre y valor correctos.
    - Si no es así, cambia el nombre/valor y vuelve a intentarlo.
    - Si es correcto, sigue leyendo.
  - Verifica que Google Colab tenga permiso para acceder a Google Drive.
   - Si no es así, debería solicitarse, concede el permiso a Google Drive si quieres que el servidor funcione.
   - Si tiene permiso, verifica la terminal en busca de errores y pégalos en la [Página de Issues](https://github.com/Prozoon700/700s-MineColabs/issues).
- ¿Cómo me hago operador del servidor?
  - Escribe en la terminal el siguiente comando: `op {tu-nombre}`
- ¿Cuánto tiempo permanecerá encendido mi servidor?
  - Comúnmente, un servidor puede estar un máximo de 12 horas después de ser detenido si alguna característica externa está actuando en el tiempo de inicio del servidor.
  - Puedes verificar esto siguiendo estos pasos:
  - `Menú Superior` > `Entorno de Ejecución` > `Ver Recursos` > `Debajo del menú de título o el gráfico de recursos`

# :crystal_ball: El Futuro del Proyecto
- En primer lugar, me gustaría tener algunas personas que quieran probar las versiones beta para que pueda encontrar fácilmente los errores y solucionarlos (y también puedo tocar hierba🌿).
- El proyecto debería y debe continuar, así que haré mi mejor esfuerzo para actualizarlo y resolver los errores que tú y yo encontremos.
- Intentaré crear una verdadera Interfaz de Usuario (web) donde puedas controlar y gestionar las cosas mucho más fácilmente. Estará basada en el Panel de Pterodactyl.
