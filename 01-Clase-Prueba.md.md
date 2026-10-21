# Mi primera clase de programación

Esta es una prueba de mi cuaderno digital sincronizado con GitHub.

```java
public class HolaMundo {
    public static void main(String[] args) {
        System.out.println("¡Hola GitHub!");
    }
}
```

![[Pasted image 20261021141720.png]]

--- ### Paso 3: Probar la inserción de imágenes 
1. En tu computadora, toma una captura de pantalla de cualquier cosa (presionando `Impr Pant` o la combinación `Windows + Shift + S`). 
2. Regresa a tu nota en Obsidian y presiona **`Ctrl + V`** (pegar). 
3. Verás que la imagen aparece inmediatamente en tu hoja y el archivo se guarda solo dentro de tu carpeta `img`. 
 
--- ### Paso 4: Subir los cambios a GitHub inmediatamente 
No necesitamos esperar 10 minutos para ver si funciona. Haremos el guardado manual de prueba: 
1. Presiona las teclas **`Ctrl + P`** en tu teclado (se abrirá una barra de búsqueda en la parte superior de Obsidian). 
2. Escribe en esa barra: `Git: Commit all changes and push`. 
3. Presiona la tecla **Enter**. 
 
--- ### Paso 5: Verificar en GitHub 
1. Abre tu navegador web e ingresa a tu repositorio: `[https://github.com/Yelanyels/apuntes-programacion](https://github.com/Yelanyels/apuntes-programacion)` 
2. Recarga la página (presionando `F5`). 
 
¡Ahí verás tu archivo `01-Clase-Prueba.md` y la carpeta `img` con tu imagen completamente guardados! 
Sigue estos pasos con calma y dime si lograste ver el archivo subido a tu GitHub.

1. En la primera captura (Imagen 1): ¡Ya se guardó solo!
   En la esquina superior derecha de Obsidian te apareció la notificación emergente:   
    Committed 1 file
    Pull: Everything is up-to-date   
   Esto confirma que el complemento automático guardó tu archivo sin que tengas que presionar nada. Además, abajo a la derecha de la barra de estado se lee: Git: committed 1 file.   
2. En la segunda y tercera captura (Imágenes 2 y 3): Por qué dice "No se encontraron comandos"
    Cuando presionas Ctrl + P, estás abriendo el buscador interno de Obsidian.En la Imagen 2, escribiste Git: Commit all changes and push.En la Imagen 3, escribiste Commit all changes and push.En las versiones recientes del plugin Git, ese comando largo se llama de forma ligeramente distinta o simplificada.Para ejecutarlo manualmente desde Ctrl + P, prueba escribir únicamente:PlaintextGit: Push
o también:PlaintextGit: Commit
Al escribir solo Git: verás la lista de todos los comandos de Git disponibles.Resumen:No necesitas preocuparte por usar el buscador de comandos a diario. Como vimos en la primera imagen, Obsidian ya guarda y sincroniza automáticamente cada 10 minutos en segundo plano hacia GitHub.   