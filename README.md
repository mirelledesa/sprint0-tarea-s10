# Registro de usuarios   
**Descripció**: Breu explicació de l'objectiu.  

## 🛠 Tecnologies  
- Frontend: React, Tailwind  
- Backend: Java, MongoDB  

## contexto 
""Como usuario de la tienda online, quiero poder registrarme con mi correo electrónico y contraseña para crear una cuenta." 

### criterios de aceitacion
- se validam em tiempo real que o formato de email seam validos.
- la contrasenha necessitam ter minimo 6 digitos incluindo letras e numeros
- se validam em tiempo real que as senhas coincidam
- el usuario necessiatar confirmar el email enviado

### Escenarios de Prueba con Gherkin
#### Registro com exito
- Ao clicar no formulario eletronico ao poner el formato de email "email@exemple.com" sera confirmado o formato valido.
- o usuario preenchera a compo de senha e confirmação de senha com as caracteries obrigatorias "exemp098".
- o sistema validar a compatibilidade dos campos e aprova.
- o usuario clica em "registrame" e exibi a mensagem "conta criada, por favor verificar o seu email eletronico".
- o usuaria confirma clica em "confirmar" no email e acessa a plataforma.
  
#### Tentativa de registra 
 Ao clicar no formulario eletronico ao poner el formato de email "email@exemple.com" sera confirmado o formato valido.
- o usuario preenchera a compo de senha e confirmação de senha sem as caracteries obrigatorias "exemplo".
- o sistema exibi a mensagem na tela "incluir letras e numeros".

## Desglose de Tareas
-Maquetar formulario de registro
HTML:
`<form>`, `<fieldset>`, `<legend>`, `<label>`, `<input type="email">`, `<input type="password">`, `<input type="checkbox">`, `<button type="submit">`
CSS:
`display`, `max-width`, `margin`, `padding`, `border-radius`, `:focus`, `:hover`, `@media`
JavaScript:
`querySelector()`, `addEventListener()`, `preventDefault()`, `.value`, `classList`
-Subir formalio na web 
-Criar o arquivo index.html e estruturar o formulário.
-Criar o arquivo style.css e aplicar o design visual e a responsividade.
-Criar o arquivo script.js para capturar os dados dos campos e fazer as validações iniciais.
-Criar e configurar o Banco de Dados
-Hospedar o Front-End
-Hospedar o Back-End e Banco de Dados
-Testar o cadastro com o site já publicado na internet.

  
## 📸 Demo  
