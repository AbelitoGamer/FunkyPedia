# Música y Chart

Para empezar con el proceso de creación, primero necesitas haber creado tu nivel desde el menú. Puedes hacerlo fácilmente desde `Crear > Nuevo proyecto`. Después de nombrarlo, este aparecerá en la lista y podrás seleccionarlo para entrar al editor.

Como en todo juego rítmico, un nivel tiene **dos elementos principales** que guían su jugabilidad: una **canción** y un **chart** que la acompaña. Así pues, el primer paso para crear esta adaptación de `Lit Up` será añadir la canción y su respectivo chart.

Al entrar por primera vez a tu nivel, verás una pantalla mayormente vacía con un botón que te pedirá seleccionar la música. A esta pantalla la llamaremos `Level Data`. Al pulsar el botón, se abrirá tu explorador de archivos, desde donde deberás buscar la carpeta donde colocaste los contenidos del archivo ZIP de assets del nivel. Una vez localizada, entra y verás tres carpetas. La que nos interesa en este momento es la carpeta **Music**. Selecciona el archivo `Lit Up.ogg`.

Después de eso, la app te pedirá introducir los valores de **BPM** y **NPB** para la canción. Por suerte, podemos ignorar estos valores y simplemente pulsar **OK**, ya que importaremos un chart que sobrescribirá esta información con los valores correctos para la canción.

Aparecerán **cuatro nuevos botones** en la pantalla, pero por ahora solo nos interesa este:

![Chart editor button](assets/images/chart-editor-button.png)

Pulsar este botón te llevará al `Chart Editor`. Nuestro siguiente paso será **importar el chart**, para que el juego pueda leer toda su información, incluyendo el mapeo y otros datos importantes como el BPM que omitimos antes. Para hacerlo, pulsa el botón de importar desde esta misma pantalla:

![Chart import button](assets/images/chart-import-button.png)

Se abrirá un submenú desde el cual deberás pulsar el botón que dice **"(import .json)"**. Esto abrirá nuevamente tu explorador de archivos. El chart se encuentra en la misma carpeta donde encontraste la música del nivel, y su nombre es `Lit Up Chart.json`. Una vez lo selecciones, notarás que el marcador de posición de la canción se mueve más rápido. Esto se debe a que ahora el juego ha cargado el BPM real de la canción, y también ha calculado el **NPB ideal** para su chart.

¡Listo! Ahora tu nivel cuenta con la canción y el chart original, ambos importados y funcionando correctamente.

Si lo deseas, puedes revisar el chart usando los botones de `ENEMIGO` y `JUGADOR` para alternar entre sus respectivas secciones. También puedes usar la barra de desplazamiento a la derecha para avanzar rápidamente en la canción, o el botón de seguimiento para que el marcador se mueva en sincronía con la reproducción de la música.

Si quieres probar tu canción, pulsa el botón de retroceso para volver a la pantalla de `Level Data` y selecciona el botón de **Jugar**. Como todavía no hemos importado nuestros assets visuales, el juego utilizará los suyos por defecto, lo cual será suficiente para que puedas jugar la canción con algo más que una pantalla negra.

Sigue al [siguiente paso](01-02-importar-los-graficos.md) para aprender a importar todos los graficos que usaremos en nuestro nivel.