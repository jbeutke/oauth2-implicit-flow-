# oauth2-implicit-flow-
OAuth 2.0 Implicit Flow - Lab

1. Clonar este repositorio:
```
git clone https://github.com/jbeutke/oauth2-implicit-flow-.git
```

2. Abrir archivo ./server.js.
   ```
   
   > En la seccion debajo de la linea '//Step 2: Exchange the code for a token' modificar las constantes con los siguientes valores:
   ```
    const Token_Endpoint = `http://localhost:8080/v1/oauth/tokens`;
    const Grant_Type = 'authorization_code';
    const Code = req.body.code;
    const Redirect_Uri = 'http://localhost:8000/give/me/the/code';
    const Scope = 'read';
    
    Estos son los parametros que requiere el Authorization Server para entregar un access_token. En base a estos parametros se armara un request para solicitarlo.

   ```


2. Desde la terminal, ingresar a la carpeta 'oauth2-implicit-flow-' y ejecutar 'npm install'.

3. Ejecutar 'npm start'

4. Ingresar a http://localhost:8000 desde el navegador.

5. Seguir las instrucciones.
