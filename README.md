# Servidor WEB/REST con ExpressJS + Mongoose + Passport-session + ConnectMongo + Passport-Local, persistencia en MongoDB Local, process, env, args, yargs, proceso hijos, BALANCE DE CARGA con PM2 y NGINX, ahora agregamos "compresion" tambien logger con 'log4js' y se prueba el server con 'artillery' (Todo esta ultima parte la saco para poder hacer el deploy en Heroku)

### Para instalar los paquetes necesarios usar:

``` npm install ```

### Para usar en local entrar a cada carpeta según el interes y ejecutar:

``` npm run dev ``` or ``` npm start ```

### Nota 1: Usar mongo local o atlas
### Nota 2: Para el puerto del server usar el parametro -p 3000 en package.json, si no se pasa parametro del puerto lo busco en .env en la variable PORT, y si no esta definida usara por defecto 8080
### Nota 3: Para comprobar el child_process consultar el endpoint /api/randoms?cant=500000000 esto genera un proceso muy grande y no bloquea el proceso del servidor que se puede seguir usando, probar entrando al localhost:port al "/"

### Para poder deployar en Heroku saco toda la parte de Testing pero dejo logger, tambien cambio de MongoLocal a MongoDB Atlas configurando las variables de entorno correspondientes.
