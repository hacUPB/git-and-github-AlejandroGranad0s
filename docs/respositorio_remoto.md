# Cómo crear un repositorio remoto en GitHub y sincronizarlo con el repositorio local

1. **Crear el repositorio remoto en GitHub:**
   - Ingresa a [GitHub](https://github.com/) y accede con tu cuenta.
   - Haz clic en el botón "New" o "Crear repositorio".
   - Escribe el nombre del repositorio y una breve descripción.
   - Elige si el repositorio será público o privado.
   - Haz clic en "Create repository".

2. **Vincular el repositorio local con el remoto:**
   - Copia la URL del repositorio remoto (por ejemplo, `https://github.com/usuario/nombre-repositorio.git`).
   - En la terminal, dentro de la carpeta de tu proyecto local, ejecuta:
     ```
     git remote add origin https://github.com/usuario/nombre-repositorio.git
     ```

3. **Subir los cambios locales al repositorio remoto:**
   - Realiza un commit si no lo has hecho:
     ```
     git commit -m "Primer commit"
     ```
   - Sube los archivos al repositorio remoto:
     ```
     git push -u origin master
     ```
     (En algunos casos, la rama principal puede llamarse `main` en vez de `master`).

4. **Sincronizar cambios entre local y remoto:**
   - Para descargar los cambios del repositorio remoto:
     ```
     git pull origin master
     ```
   - Para subir nuevos cambios locales:
     ```
     git push origin master
     ```

Con estos pasos, tu repositorio local estará sincronizado con el repositorio remoto