# oauth2-implicit-flow-
OAuth 2.0 Implicit Flow - Lab

1. Clonar este repositorio:
```
git clone https://github.com/jbeutke/oauth2-implicit-flow-.git
```

2. Abrir archivo 'views/index.ejs'.
   > En la linea 56 modificamos el href para que cuando hagamos click en el boton, le pida un token al servidor de autorizacion.:

   ```

                            <a href="http://localhost:8080/web/authorize?response_type=token&client_id=test_client_1&redirect_uri=http://localhost:8000/give/me/the/access/token&state=ZGSwKqq97LP2h6SI" class="btn btn-primary">Go to the authorization server</a>

    
    Estos son los parametros que requiere el Authorization Server para entregar un access_token. En base a estos parametros se armara un request para solicitarlo.

   ```


2. Desde la terminal, ingresar a la carpeta 'oauth2-implicit-flow-' y ejecutar 'npm install'.

3. Ejecutar 'npm start'

4. Ingresar a http://localhost:8000 desde el navegador.

5. Seguir las instrucciones.
