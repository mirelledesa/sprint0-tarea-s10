# Registro de usuarios   
**Descripción**: Creación de la interfaz y la lógica necesaria para que los nuevos clientes puedan crear una cuenta en la tienda online de forma segura y accesible.

## Contexto  
> **Como** usuario de la tienda online,  
> **quiero** poder registrarme con mi correo electrónico y contraseña,  
> **para** crear una cuenta y realizar compras.

### Criterios de aceptación
* Se valida en tiempo real que el formato del correo electrónico sea válido.
* La contraseña debe tener un mínimo de 6 caracteres, incluyendo letras y números.
* Se valida en tiempo real que la contraseña y la confirmación de la contraseña coincidan.
* El usuario debe confirmar su cuenta a través de un enlace enviado a su correo electrónico para activar el acceso.

### Escenarios de Prueba con Gherkin

#### Escenario 1: Registro exitoso
* **Dado que** el usuario se encuentra en el formulario de registro,
* **Cuando** introduce un correo válido como "email@ejemplo.com", completa los campos de contraseña y confirmación con un valor válido como "ejemp098" y hace clic en el botón "Registrarme",
* **Entonces** el sistema valida que los datos coinciden con los criterios, procesa el registro y muestra en pantalla el mensaje: *"Cuenta creada. Por favor, verifica tu correo electrónico"*.
* **Y cuando** el usuario revisa su bandeja de entrada y hace clic en el enlace de "Confirmar", el sistema activa la cuenta y le permite acceder a la plataforma.

#### Escenario 2: Intento de registro con contraseña inválida
* **Dado que** el usuario se encuentra en el formulario de registro y ha introducido un correo electrónico válido,
* **Cuando** completa los campos de contraseña y confirmación con un formato incorrecto (por ejemplo, sólo letras: "ejemplo"),
* **Entonces** el sistema valida los datos en tiempo real, bloquea el envío del formulario y muestra un mensaje de error en la pantalla que dice: *"La contraseña debe incluir letras y números"*.


## Desglose de Tareas

### Tarea 1: Maquetar el formulario de registro 
* **HTML**: Crear el archivo `index.html` utilizando las etiquetas `<form>`, `<fieldset>`, `<legend>`, `<label>`, `<input type="email">`, `<input type="password">`, `<input type="checkbox">` y `<button type="submit">`.
* **CSS**: Crear el archivo `style.css` aplicando diseño visual y responsividad con las propiedades `display`, `max-width`, `margin`, `padding`, `border-radius`, `:focus`, `:hover` y `@media`.
* **JavaScript**: Crear el archivo `script.js` para capturar los datos de los campos y realizar las validaciones en tiempo real utilizando `querySelector()`, `addEventListener()`, `preventDefault()`, `.value` y `classList`.

### Tarea 2: Creación del Servidor y Base de Datos
* Crear y configurar la Base de Datos para almacenar de forma segura las credenciales de los usuarios.
* Desarrollar la lógica del servidor para recibir los datos del formulario, validar los requisitos e iniciar el proceso de envío del correo de confirmación.

### Tarea 3: Despliegue y Publicación en la Web 
* Alojar y desplegar el Front-End en producción.
* Alojar y desplegar el Back-End y la Base de Datos en la nube.
* Realizar pruebas de extremo a extremo con el sitio ya publicado en internet para asegurar el correcto funcionamiento del flujo de registro.

Notion: https://app.notion.com/p/392f75f8a4a380948a1dc88c8853178c?source=copy_link


## 📸 Demo
