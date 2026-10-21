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



