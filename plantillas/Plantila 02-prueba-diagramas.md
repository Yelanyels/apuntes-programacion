# 📌 Módulo 01: Flujo de Autenticación de Usuarios
* **Tecnología:** Java / Spring Boot / MySQL
* **Estado:** Apunte de clase

> [!NOTE] 📋 Objetivos de la Clase
> Comprender el proceso de validación de credenciales, el flujo de decisiones y el almacenamiento en la base de datos.

---

## 1. Diagrama de Proceso (Flujo de Login)

> [!ABSTRACT] 📐 Diagrama de Flujo del Sistema
> ```mermaid
> graph TD
>     A[Inicio: Usuario ingresa credenciales] --> B{¿Usuario y Password correctos?}
>     B -- Sí --> C[Generar Token JWT]
>     B -- No --> D[Retornar Error 401 Unauthorized]
>     C --> E[Guardar Sesión en Base de Datos]
>     E --> F[Fin: Acceso Permitido]
> ```

---

## 2. Estructura de la Base de Datos

> [!DATABASE] 📊 Entidades Relacionadas
> ```mermaid
> erDiagram
>     USUARIO ||--o{ SESION : genera
>     USUARIO {
>         int id PK
>         string username
>         string password_hash
>     }
>     SESION {
>         int id PK
>         string token
>         date fecha_inicio
>     }
> ```

---

## 3. Ejemplo de Código en Backend

> [!INFO] 💻 Método de Validación en Java
> **Descripción:** Lógica principal para consultar al usuario en la base de datos.
> ```java
> public boolean autenticarUsuario(String username, String password) {
>     Usuario user = usuarioRepository.findByUsername(username);
>     if (user != null && user.getPassword().equals(password)) {
>         return true; // Credenciales válidas
>     }
>     return false; // Error de autenticación
> }
> ```

---

## 4. Notas y Advertencias

> [!WARNING] ⚠️ Regla de Seguridad
> Nunca guardes contraseñas en texto plano. Usa siempre un algoritmo de encriptación como **BCrypt** antes de registrar el usuario.

> [!SUCCESS] 💡 Buena Práctica
> Configura un tiempo de expiración corto para los tokens de sesión para proteger la cuenta.