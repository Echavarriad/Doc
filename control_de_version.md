### Conexion ssh
- se obtiene .pem
- se abre la consolo cmd
- se ejecuta el comando ``` ssh -i C:\ruta\de\archivo\bibliotech.pem _____user@20.92.**.****```
- se acepta la conexión por pirmera vez
> una vez hecho estos pasos se abrira la terminal de servidor ubuntu 


### configurar repositorio 
### permisos directorio /var/www
```
> sudo chmod -R 775 /var/www
> sudo chown -R www-data:www-data
> Cd /var/www/
```
> Git clone repositorios credenciales para autenticar entregadas por bibliotech
```
> Cd bibliotech
```
## Permisos archivos y directorios
```
sudo find . -type d -exec chmod 755 {} \;
 sudo find . -type f -exec chmod 644 {} \;
Composer install 
Yarn install 
Yarn run build 
```

> Una ves el proyecto ya este corriendo en estado de producción con los permisos se podrá controlar lo cambios en el proyecto con el repositorio en gitlab a través de los siguientes comandos.

- Se dirige al lugar donde se encuentra el proyecto en este caso es: /var/www/proyecto , dentro de este usaremos lo siguientes comando si ya está el origin del repositorio 

```
git pull
```

- el git pedira crendeiclaes, para este paso es necesario ingresar al gitlab y generar un token de autentificaion desde el perfil de gitlab 
