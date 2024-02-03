# Ruta de servidor
## Oportuna red
### Instalación de Software Común o configuracion entorno base

### Actualizar el Sistema:
```
> sudo yum update -y
```
### El comando "sudo yum update -y" se utiliza para realizar una actualización completa del sistema instalando las últimas versiones de los paquetes disponibles. Es una buena práctica mantener los sistemas actualizados para asegurarse de que tengan las últimas correcciones de seguridad y mejoras.

### Instalar Utilidades:
```
> sudo yum install -y vim wget curl
```
### El comando "sudo yum install -y vim wget curl" instalará los paquetes Vim (editor de texto), wget (herramienta de descarga) y curl (herramienta de transferencia de datos) en el sistema.

### Instalar Git:
```
> sudo yum install -y git
```

### El comando "sudo yum install -y git" instalará el paquete Git en el sistema, permitiendo que los usuarios realicen operaciones de control de versiones en sus proyectos. Git es una herramienta esencial para desarrolladores y equipos de desarrollo de software que facilita la colaboración y el seguimiento de cambios en el código fuente.


### Instalar Python 3 y pip:
```
> sudo yum install -y python3

>sudo yum install -y python3-pip
```

### Después de ejecutar esta instrucción, tendrás Python 3 instalado en tu sistema y podrás utilizar el intérprete de Python 3 (python3) y otras herramientas asociadas, como pip3 (el gestor de paquetes para Python 3), para instalar paquetes y bibliotecas adicionales. 

### PIP: Al ejecutar esta instrucción, se instalará pip para Python 3, lo que te permitirá instalar fácilmente paquetes y bibliotecas de Python adicionales en tu sistema utilizando el comando pip3.

```
> pip3 install paquete_python
```

### Instalar NVM:
```
> sudo yum update -y
> git --version
if(git)
> curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
else
> sudo yum install -y git
```
### Estos comando descargará el script de instalación de NVM y lo ejecutará. Asegúrate de utilizar la versión más reciente de NVM; puedes verificar la última versión en el 
### Recargar el perfil del shell:
```
> source ~/.bashrc
```
### Verificar la instalación de NVM:
```
> nvm --version
```
### Esto mostrar la versión de NVM instalada.

### Instalar Node.js:
```
> nvm install <version>
```
### instala la version de nodejs con el npm con la version respetiva 
### Usar version de Node.js:
```
> nvm use <version>
```
### selecciona una de las versiones instaladas dependiendo del requicito 
### Instalar PHP:
```
> sudo amazon-linux-extras install php7.4
> sudo amazon-linux-extras install php8.0
```

### La instrucción "sudo amazon-linux-extras install phpmayor.menor>" intenta instalar todas las versiones disponibles de PHP proporcionadas por los extras de Amazon Linux.

### Version de php:
```
>php -v
```
### Para gestionar varias versiones de PHP, puedes utilizar el comando 'alternatives':
```
>sudo alternatives --config php
```
### Instalar Docker:
```
> sudo amazon-linux-extras install docker
> sudo service docker start
> sudo usermod -aG docker ec2-user
```
### La instrucción sudo amazon-linux-extras install docker se utiliza en Amazon Linux para instalar el paquete de Docker a través de Amazon Linux Extras. Amazon Linux Extras es un mecanismo que facilita la instalación y el manejo de software adicional en sistemas Amazon Linux al proporcionar paquetes de software actualizados y gestionados por Amazon.
### Imágenes de Docker:
1. Versiones Etiquetadas:
 - Utiliza versiones etiquetadas para tus imágenes de Docker (por ejemplo, miapp:1.0). Esto facilita el seguimiento de las versiones y garantiza la reproducibilidad.
2. Dockerfile Eficiente:
  - Crea Dockerfiles eficientes y optimizados para reducir el tamaño de las imágenes. Usa capas de manera efectiva y elimina cualquier elemento innecesario.
3. Seguridad:
  - Escanea tus imágenes en busca de vulnerabilidades utilizando herramientas como Clair, Anchore o Trivy.
4. Imagen Base Oficial:
- Utiliza imágenes base oficiales siempre que sea posible. Estas imágenes están bien mantenidas y son generalmente seguras.
5. Contexto de Construcción:
  -Limita el contexto de construcción al mínimo necesario al construir imágenes. Esto mejora el rendimiento y evita la inclusión de archivos innecesarios.
6. Almacenamiento Privado:
- Considera el uso de un registro de Docker privado para almacenar imágenes sensibles o específicas de tu organización.

### Contenedores:
1. Nombres Significativos:
- Asigna nombres significativos a tus contenedores para facilitar la identificación. Puedes usar la opción --name al iniciar un contenedor.
2. Persistencia de Datos:
- Utiliza volúmenes o enlaces para persistir datos que necesitan sobrevivir al ciclo de vida de un contenedor.
3. Recursos Limitados:
- Asigna límites de recursos (CPU, memoria) a tus contenedores para evitar que consuman demasiados recursos del sistema.
4. Redes Aisladas:
- Usa redes aisladas para separar contenedores y garantizar la independencia funcional.
5. Monitoreo y Registro:
- Implementa soluciones de monitoreo y registro para evaluar el rendimiento y rastrear eventos dentro de los contenedores.
6. Escalabilidad Horizontal:
- Diseña tus aplicaciones para ser escalables horizontalmente mediante la ejecución de múltiples contenedores replicados.
7. Gestión de Estado:
- Externaliza el estado de tu aplicación fuera del contenedor siempre que sea posible. Esto facilita la actualización y reemplazo de contenedores sin pérdida de datos.
8. Salud del Contenedor:
- Utiliza la opción "--healthcheck" al construir imágenes para especificar un comando que verifica la salud del contenedor.

### Instalar Apache:
```
> sudo yum install -y httpd
```
### El comando "sudo yum install -y httpd" instalará el servidor web Apache en tu sistema. Una vez instalado, puedes iniciar y habilitar el servicio para que se inicie automáticamente al arrancar el sistem
### Instalar Nginx:
```
> sudo amazon-linux-extras install nginx1.12
```
### El comando "sudo amazon-linux-extras install nginx1.12" se utiliza en sistemas basados en Amazon Linux para instalar la versión específica 1.12 de Nginx a través de Amazon Linux Extras. Esto permite instalar y gestionar software adicional de manera eficiente en Amazon Linux.

### Apache HTTP Server y Nginx son dos de los servidores web más populares utilizados para alojar sitios web y aplicaciones. Ambos son potentes, pero tienen diferencias en su arquitectura, rendimiento y características. Aquí hay una comparación general:

# Apache HTTP Server:
## Pros:
1. Soporte Módular:
- Apache es conocido por su arquitectura modular, lo que permite la incorporación y configuración de módulos adicionales para ampliar su funcionalidad.
2. Soporte .htaccess:
- Apache utiliza archivos .htaccess para la configuración a nivel de directorio, lo que facilita la implementación de configuraciones específicas para diferentes directorios y permite a los usuarios cambiar configuraciones sin acceso al archivo de configuración principal.
3. Documentación Extensa:
- Apache tiene una documentación exhaustiva y una comunidad activa, lo que facilita encontrar información y soluciones a problemas comunes.
## Contras:
1. Uso de Recursos:
- En comparación con Nginx, Apache puede consumir más recursos en entornos con grandes cantidades de conexiones simultáneas.
# Nginx:
## Pros:
1. Rendimiento y Escalabilidad:
- Nginx está diseñado para ser ligero y escalable, lo que lo hace eficiente en el manejo de muchas conexiones simultáneas con un bajo consumo de recursos.
2. Manejo de Eventos Asíncronos:
- Nginx utiliza una arquitectura basada en eventos asíncronos, lo que le permite manejar un gran número de conexiones concurrentes sin consumir demasiados recursos.
3.Proxy Inverso y Balanceo de Carga:
- Nginx brilla en funciones como proxy inverso y balanceo de carga, siendo una opción popular para servidores que actúan como pasarelas para aplicaciones web.
## Contras:
1. Configuración más Compleja:
- La configuración de Nginx puede parecer menos intuitiva para algunos usuarios en comparación con Apache, especialmente para aquellos que están más familiarizados con la sintaxis de configuración de Apache.
2. Soporte Limitado .htaccess:
- A diferencia de Apache, Nginx no admite archivos .htaccess, lo que puede hacer que las configuraciones a nivel de directorio sean menos flexibles para algunos usuarios.
- 
# Elección entre Apache y Nginx:
Escenario de Uso:

Apache es una opción sólida para entornos donde la flexibilidad y el soporte de módulos son críticos. Nginx brilla en situaciones de alto rendimiento y manejo eficiente de muchas conexiones simultáneas.
Requerimientos de Recursos:

Si estás gestionando un servidor con recursos limitados y necesitas alto rendimiento, Nginx puede ser una mejor opción. Para proyectos más pequeños o aquellos que dependen de la flexibilidad de módulos de Apache, Apache puede ser preferible.
Conocimientos y Preferencias Personales:

A menudo, la elección entre Apache y Nginx también depende de la familiaridad y preferencias personales del administrador del sistema o desarrollador.
### Configurar Virtual Host:
```
> /etc/nginx/conf.d/
```

### Configuración Adicional
### Seguridad

### Configurar firewalls, SELinux, y otras medidas de seguridad según las necesidades con la consola de AWS


### Documentación y Mantenimiento:
### Documentación:
### Crear documentación detallada para la configuración del servidor y cada aplicación.

### Mantenimiento Regular:
### Establecer procedimientos para actualizaciones y mantenimiento regular.
