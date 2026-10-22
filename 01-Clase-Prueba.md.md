# Mi Creación paso a paso

Esta es una prueba de mi cuaderno digital sincronizado con GitHub.

```java
public class HolaMundo {
    public static void main(String[] args) {
        System.out.println("¡Hola GitHub!");
    }
}
```

![[Pasted image 20261021141720.png]]

¡Excelente elección! La combinación de **Obsidian + MkDocs** te dará lo mejor de ambos mundos: un entorno supercómodo para tomar notas a diario con imágenes y código, y la generación automática de un libro/sitio web profesional alojado gratis en tu GitHub.

Vamos a configurarlo **paso a paso**. En esta **Fase 1** dejaremos listo tu repositorio en GitHub y tu cuaderno en Obsidian con sincronización automática.

Paso 1: Crear el repositorio en GitHub

1.Entra a tu cuenta de **GitHub** y haz clic en el botón verde **"New"** (o en el ícono `+` arriba a la derecha > **New repository**).

2.Llena los siguientes datos:
 - **Repository name:** `apuntes-programacion` (o el nombre que prefieras para tu cuaderno/libro).
    
- **Description:** (Opcional) _Mi cuaderno de notas y libro digital de clases de programación._
    
- **Public / Private:** Elige **Public** (si quieres publicarlo luego con MkDocs) o **Private** (puedes cambiarlo después).
    
- **Initialize this repository with:** Marca la casilla **Add a README file**.

3.Haz clic en **Create repository**.

![[Pasted image 20261021152926.png]]

¡Excelente! Veo que tu repositorio **`apuntes-programacion`** ya está creado perfectamente en tu GitHub.

El siguiente paso es **descargar (clonar) ese repositorio en tu computadora** y conectarlo con **Obsidian** para empezar a escribir tus clases. Vamos con ello paso a paso:

**Paso 2: Clonar el repositorio en tu computadora**

1.Abre la terminal de tu computadora (puede ser Git Bash, CMD o PowerShell).

2.Entra a la carpeta donde te guste guardar tus proyectos o documentos (por ejemplo, escribe `cd Documentos` y presiona Enter).

3.Copia y pega el siguiente comando para clonar tu repositorio recién creado:
![[Pasted image 20261021153155.png]]
git clone https://github.com/Yelanyels/apuntes-programacion.git

Esto descargará la estructura de tu repositorio y creará una carpeta llamada `apuntes-programacion` en tu PC.

![[Pasted image 20261021153420.png]]


Aquí tienes los enlaces e información para obtener ambas aplicaciones antes de continuar:

   Links de descarga e instalación
   Obsidian (Programa para tomar notas):

   **Sitio oficial de descarga:**  [https://obsidian.md/download](https://obsidian.md/download)
   
MkDocs (Generador de sitio web / Libro digital):

MkDocs no es un programa instalable tradicional con ejecutable `.exe`, sino una herramienta que se instala mediante comandos de Python.

Por ahora **no necesitas instalar MkDocs**, ya que primero estructuraremos tus apuntes e imágenes dentro de Obsidian. Cuando tus notas estén creadas y sincronizadas en GitHub, usaremos un comando sencillo de Python o las propias acciones automáticas de GitHub (_GitHub Actions_) para publicar el libro digital.

Una vez que hayas descargado e instalado **Obsidian**, puedes proceder con los pasos que mencionaste:

1.**Abre Obsidian** en tu computadora.
![[Pasted image 20261021154031.png]]

Puedes dejar seleccionada la opción que ya tienes marcada: **"Solo para mí. (ACER)"**.

Es la opción recomendada porque se instala de forma estándar en tu perfil de usuario y no te pedirá permisos de administrador para futuras actualizaciones.

Simplemente haz clic en el botón **"Siguiente >"** para continuar con la instalación.

**Una vez dentro de Obsidian:***

- Haz clic derecho en el panel izquierdo y crea una nueva carpeta llamada **`img`**.
    
- Ve a la **Configuración de Obsidian** (el engranaje ⚙️ abajo a la izquierda).
    
- Entra a **Files and links** (Archivos y enlaces).
   
- En el menú lateral, entra a **Archivos y enlaces** (Files and links).

- Busca la opción **Ubicación predeterminada para nuevos adjuntos** (Default location for new attachments) y cámbiala a:

![[Pasted image 20261021154623.png]]

En esa casilla que remarcaste en rojo (**Ubicación predeterminada para los archivos adjuntos nuevos**), debes hacer lo siguiente:

Haz clic donde dice **"Carpeta de la bóveda"** y selecciona la opción: **"En la carpeta especificada a continuación"**.

Al seleccionar eso, aparecerá un nuevo campo de texto debajo llamado **"Ruta de la carpeta de archivos adjuntos"**. Ahí escribe:
![[Pasted image 20261021154741.png]]
img
(Asegúrate de haber creado primero la carpeta `img` en el panel izquierdo de Obsidian para que la reconozca).

![[Pasted image 20261021154839.png]]

Paso siguiente: Activar e instalar el plugin Obsidian Git

Ahora activaremos la sincronización automática con tu repositorio de GitHub:

1.En el menú lateral izquierdo de esa misma ventana de Preferencias, haz clic en **Complementos comunitarios**.

![[Pasted image 20261021163200.png]]

Haz clic en el botón morado que dice **"Salir del modo restringido"**.

Eso desactivará la protección inicial y desbloqueará la tienda de complementos de Obsidian.

Inmediatamente después de hacer clic:

1.Te aparecerá un botón llamado **"Explorar"** (o _Browse_). Haz clic en él.

![[Pasted image 20261021163549.png]]

¡Excelente! Ya saliste del modo restringido correctamente.

Ahora realiza estos sencillos pasos:

1.Haz clic en el botón **Buscar** que está a la derecha de _"Complementos creados por la comunidad"_.

2.Escribe únicamente:
![[Pasted image 20261021164140.png]]
Git

![[Pasted image 20261021164256.png]]

¡Eso es! La **primera tarjeta** que te aparece arriba a la izquierda, la que se llama simplemente **`Git`** (Por Vinzent, con 3.3M de descargas) es la correcta.

Sigue estos pasos sencillos:

1.Haz clic en esa primera tarjeta **Git**.

2.En la pantalla que se abre, haz clic en el botón **Instalar**.

3.Cuando termine de descargar, ese mismo botón cambiará a **Activar**. Haz clic en **Activar**.

Ajustes finales de sincronización automática

Una vez activado:

1.Vuelve a **Preferencias** (engranaje ⚙️) y abajo del todo en la barra lateral izquierda busca y haz clic en **Git** (debajo de _Opciones de complementos_).

![[Pasted image 20261021164538.png]]

¡Excelente! Ya estás en el panel de configuración de Git.   

Para configurar los tiempos de guardado automático hacia tu GitHub, haz lo siguiente:

1.Haz clic en la primera opción de la lista que se llama Automatic (Scheduled commit, pull, and push routines).   

![[Pasted image 20261021164725.png]]
![[Pasted image 20261021164817.png]]


Paso 1: Configurar los tiempos automáticos (En la pantalla donde estás)

En la ventana que tienes abierta en tu pantalla:

1.Busca la opción que dice **`Auto commit-and-sync interval (minutes)`**.

- Borra el `0` y escribe: **`10`**. _(Esto guardará y subirá tus notas a GitHub automáticamente cada 10 minutos)_.

2.Un poco más abajo, busca la opción que dice **`Auto pull interval (minutes)`**.

Borra el 0 y escribe: 10. (Esto descargará cualquier cambio nuevo si abres Obsidian en otra PC).   

3.Ahora cierra esa ventana de Preferencias haciendo clic en la X que está arriba a la derecha.   

**Paso 2: Crear tu primera nota/clase de prueba

1.En la parte izquierda de Obsidian, haz clic derecho en un espacio vacío del panel de archivos y selecciona **Nueva nota** (o presiona `Ctrl + N`).

2.Ponle de nombre: `01-Clase-Prueba.md`.

3.Haz clic dentro del área blanca de la nota y escribe exactamente esto:

![[Pasted image 20261021165208.png]]
# Mi primera clase de programación

Esta es una prueba de mi cuaderno digital sincronizado con GitHub.

```java
public class HolaMundo {
    public static void main(String[] args) {
        System.out.println("¡Hola GitHub!");
    }
}
```

### Paso 3: Probar la inserción de imágenes

1.En tu computadora, toma una captura de pantalla de cualquier cosa (presionando `Impr Pant` o la combinación `Windows + Shift + S`).

2.Regresa a tu nota en Obsidian y presiona **`Ctrl + V`** (pegar).

3.Verás que la imagen aparece inmediatamente en tu hoja y el archivo se guarda solo dentro de tu carpeta `img`.

 como puedo sacar ``` esos acentos 
 alt Gr + G} ```

![[Pasted image 20261021165730.png]]

Conexión: 

![[Pasted image 20261022070313.png]]
![[Pasted image 20261022070446.png]]
![[Pasted image 20261022070409.png]]
En las imágenes que enviaste hay dos cosas importantes sucediendo:

1.En Obsidian (Imagen 2): En la barra de búsqueda de comandos (Ctrl + P), escribiste el texto entre acentos graves (`Git: Commit...`). Cuando buscas un comando, no debes incluir las comillas/acentos graves.   

2.El error de Git y tu GitHub (Imágenes 1 y 3): El error fatal: ambiguous argument 'origin/main' y la pantalla inicial de GitHub indican que tu repositorio en GitHub está completamente vacío (aún no se ha realizado el primer envío o initial commit a la rama main).   

Paso 1: Hacer el envío inicial desde la terminal (Solo se hace una vez)

1.En la barra de tareas de tu pantalla (abajo), haz clic en la ventana negra/azul que dice **`MINGW64:/c/Us...`** (o abre Git Bash/PowerShell en la carpeta de tu proyecto).

![[Pasted image 20261022070736.png]]

¡Ahí está el detalle! Viendo la imagen, estás parado en la carpeta contenedora Cuadernos y Libros de Programacion, pero el repositorio de Git que clonaste está dentro de la subcarpeta apuntes-programacion.   

Para solucionarlo, debes entrar a la subcarpeta ejecutando los siguientes comandos en esa misma ventana de Git Bash:   

Paso 1: Entrar a la subcarpeta del proyecto
Copia y pega este comando y presiona **Enter**:

![[Pasted image 20261022070950.png]]
cd apuntes-programacion

(Verás que la ruta amarilla de la terminal cambiará para incluir `/apuntes-programacion` al final).

Paso 2: Subir tus archivos a GitHub
Ahora sí, ejecuta estos comandos uno por uno (presionando **Enter** después de cada uno):

1.Agregar los archivos:
![[Pasted image 20261022071251.png]]
git add .

2.Crear el punto de guardado:
![[Pasted image 20261022071327.png]]
git commit -m "primer commit"

![[Pasted image 20261022071410.png]]

¡Excelente! Ya entraste a la carpeta correcta (`apuntes-programacion`) y la terminal reconoce la rama `(main)`.

El mensaje que ves indica que los cambios ya se confirmaron localmente, pero falta vincular y subir la rama a GitHub.

Solo ejecuta estas **dos líneas finales** en esa misma terminal (una por una):

Paso 1: Establecer la rama principal
Copia y pega este comando y presiona **Enter**:
![[Pasted image 20261022071523.png]]
git branch -M main

Paso 2: Subir todo a GitHub
Copia y pega este comando y presiona **Enter**:
![[Pasted image 20261022071556.png]]
git push -u origin main

![[Pasted image 20261022071706.png]]

¡Excelente! ¡Lo lograste con éxito!

En la pantalla de la izquierda se ve claramente en tu navegador que GitHub ya recibió tus archivos (01-Clase-Prueba.md, la carpeta de imágenes y tu configuración), y en la terminal de la derecha se confirma que el push se completó al 100% sin errores.   

Tu cuaderno digital ya está completamente operativo:

**Localmente:** Escribes tus notas, códigos y pegas imágenes en Obsidian de forma rápida y cómoda.

**Respaldo automático:** Gracias al plugin de Git que configuramos, tus apuntes se guardarán y subirán a GitHub solos cada 10 minutos.

**Manual:** Si en algún momento quieres forzar un guardado inmediato antes de cerrar la laptop, solo presionas **`Ctrl + P`**, escribes `Git: Commit all changes and push` y listo.

![[Pasted image 20261022071939.png]]






 

